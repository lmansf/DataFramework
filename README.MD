# Framework for Most Data Projects
This is a simple way to organize notebooks in data science projects that include exploring the data, feature extraction, data modeling, and finally making predictions. The components are meant to be modular in nature, so that they may be adapted to various kinds of projects in the future.

## The Setup
The workspace is broken down into 3 main notebooks:
1. Notebook 1: Exploratory Data Analysis & Feature Selection
2. Notebook 2: Training/Exploring Models
3. Notebook 3: Making Predictions

## See it In Action

In the "In Action" folder are a set of 3 notebooks, and a source csv file from a recent kaggle competition I took part in. The notebooks contain my attempt at the challenge, broken down into the categories as described below.

## Notebook 1: Exploratory Data Analysis & Feature Selection
What a mouthful. "What Matters Here" for short.
Notebook 1 takes in the raw data with the goal of determining how it should be output to the next notebook. That means
- Loading and transforming data
- identifying the key features
- Trimming anything unnecessary
- Any smaller cleanups (renames, reorganizing)

## Notebook 2: Modeling the Dataset
This is the fun part. How much performance can you get out of the models at your disposal?
- First, Load the data and transform it using the predetermined transformation steps from N1.
- Second, identify, optimize, and train all possible models of interest.
- Identify the final models, and save them to be exported for N3.

## Notebook 3: Model Predictions
And this is where it pays off. This short notebook will quickly run tests. Mine will be designed to be reused with many different kinds of models and datasets, allowing me to reuse notebooks 2 & 3 in most projects with little or no changes to them.
- First, load and transform data using the previously mentioned optimizations.
- Make predictions
- Create an exportable result file in csv format

### To Do
- Refactor notebooks 2 and 3 to be reusable templates
