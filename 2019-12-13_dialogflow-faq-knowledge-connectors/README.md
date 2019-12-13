## Question answering experiments with the Dialogflow FAQ Knowledge Connectors

Data used to perform the experiments mentioned in the Nu Echo's blog post [Question answering experiments with the Dialogflow FAQ Knowledge Connectors](<TODO>).

### Description of the files

* `corpus.csv`: Data used for testing and training (training sentences were only used for the experiment involving intents). Columns are:
  * `ID`: Unique sentence identifier.
  * `Question`: User formulated question.
  * `Exact match`: A tag that represents the Q&A pair that answers the user formulated question.
  * `Train / Test set`: Indicates if the sentence is part of the train set or the test set.
* `raw-results.tsv`: Tab-separated values file containing raw Dialogflow results. Colums are:
  * The first column indicates the sentences ID (as found in `corpus.csv`).
  * The second column contains the raw JSON result.
* `tag-definitions.csv`: Contains the data used to fill in the Dialogflow Knowledge Connector. Columns are:
  * `Tag Name`: The tag name we used to represent this Q&A pair within `corpus.csv`.
  * `Question` and `Answer`: The question & answer pair.
