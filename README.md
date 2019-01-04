# TV Scripts Generation 

# Overview
In this project, I built a Recurrent Neural Network to generate my own [Seinfeld](https://en.wikipedia.org/wiki/Seinfeld) TV scripts. The architecture uses 200 dimensions embedding layers at first, 2 stacked LSTM layers with 256 dimensions hidden state each, and a fully connected layer in the end. After model was trained, I used it to predict a new, "fake" TV script, based on patterns it recognized in this training data.

# Data
The data for this project is located [here](./data/Seinfeld_Scripts.txt), which has been crawled from the http://www.seinology.com/ website. I used part of the Seinfeld dataset of scripts from 9 seasons.

# Environment
Python: 3.6

PyTorch: 0.4.0

GPU: NVIDIA GeForce GTX 970M

Windows: 8.1

# Example Generated Script


# Deliverable

Check the [**dlnd_tv_script_generation.ipynb**](./dlnd_tv_script_generation.ipynb) for all implementation.

The [**helper.py**](./helper.py) and [**problem_unittests.py**](./problem_unittests.py)
