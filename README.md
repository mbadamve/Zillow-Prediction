Zillow’s Home Value Prediction (Zestimate) :house_with_garden:
==============================

“Zestimates” are estimated home values based on 7.5 million statistical and machine learning models that analyze hundreds of data points on each property.

The goal of this project is to predict logerror (log(Zestimate)−log(SalePrice)) using various regression models and evaluate, compare performances and use the best one for prediction.

Getting Started: :white_check_mark:
---------------

1. Download the dataset using the [link](https://www.kaggle.com/c/zillow-prize-1/data) and save the zip file using the name 'zillow-prize-1' (you can also use different name, but it needs to be updated when using the code files)
2. Install the Python packages that are listed in the requirements.txt file or if they are already installed, you are good to go

Python implementation: CPython |
Python version       : 3.8.8 |
IPython version      : 7.22.0 |
 
numpy  : 1.19.2 |
pandas : 1.2.4 |
sklearn: 0.0 |

3. Make sure Python 3.8 or above is installed. If need help, please refer [here](https://www.python.org/downloads/)

Please refer to the below Project structure to understand properly how to navigate this repo. It just takes a minute :bulb:

Project Organization
------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources. Details about data download is mentioned
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
       ├── __init__.py    <- Makes src a Python module
       │
       ├── data           <- Scripts to download or generate data
       │   └── make_dataset.py
       │
       ├── features       <- Scripts to turn raw data into features for modeling
       │   └── build_features.py
       │
       ├── models         <- Scripts to train models and then use trained models to make
       │   │                 predictions
       │   ├── predict_model.py
       │   └── train_model.py
       │
       └── visualization  <- Scripts to create exploratory and results oriented visualizations
           └── visualize.py

Results
--------

I have used HistGradientBoostingRegressor from sklearn that produced amazing results. 

![Final Result](result.png)

References
----------

1. Scikit-learn resources from https://scikit-learn.org/
2. Kaggle Community discussions

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
