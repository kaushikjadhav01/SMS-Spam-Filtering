# SMS Spam Filtering

## Installation
1. Install [Python] 3.6 and optionally create a dedicated environment
1. Clone the repository
    ```bash
    git clone https://github.com/dperdios/sms-spam-filtering
    cd sms-spam-filtering
    ```
1. Install the [Python] dependencies from `requirements.txt`
    ```bash
    pip install --upgrade -r requirements.txt 
    ```
[python]: https://www.python.org

## Dataset
We used the [SMS Spam Collection dataset][sms-dataset] proposed
by [kaggle].
> The SMS Spam Collection is a set of SMS tagged messages that have been
collected for SMS Spam research.
It contains one set of SMS messages in English of 5574 messages,
tagged acording being ham (legitimate) or spam.

For simplicity, it is also stored in this repository under `datasets/spam.csv`. 

More info on the dataset: [link][sms-dataset]

[kaggle]: https://www.kaggle.com/
[sms-dataset]: https://www.kaggle.com/uciml/sms-spam-collection-dataset

## Code
The following [Python] scripts and [Jupyter] notebooks are available:

* [data_exploration.ipynb]: Data exploration notebook.
* [example_classifier.ipynb]: Notebook providing an example of classifier
training.
* [increasing_sensitivity.ipynb]: Notebook providing an example of sensitivity
increase by dataset resampling.
* [data_exploration.py]: Produces the data exploration figures (stored under
`results/data-exploration/`).
* [classifiers_grid_search.py]: Allows to re-train the classifiers for the
different dataset resampling strategies.
The trained classifiers are stored under `results/trained-classifiers/`.
* [classifiers_scores.py]: Allows to compute the different scores on trained
classifiers (which are stored under `results/trained-classifiers/`).
* [online_learning.py]: Allows to re-run the online learning experiments.
Note that the training will only be performed if the configuration is not
already stored under `results/online-learning/`

[jupyter]: https://jupyter.org/
[data_exploration.ipynb]: https://nbviewer.jupyter.org/github/dperdios/sms-spam-filtering/blob/master/scripts/data_exploration.ipynb
[example_classifier.ipynb]: https://nbviewer.jupyter.org/github/dperdios/sms-spam-filtering/blob/master/scripts/example_classifier.ipynb
[increasing_sensitivity.ipynb]: https://nbviewer.jupyter.org/github/dperdios/sms-spam-filtering/blob/master/scripts/increasing_sensitivity.ipynb
[data_exploration.py]: scripts/data_exploration.py
[classifiers_grid_search.py]: scripts/classifiers_grid_search.py
[classifiers_scores.py]: scripts/classifiers_scores.py
[online_learning.py]: scripts/online_learning.py

