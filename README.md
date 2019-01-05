# TV Scripts Generation 

# Overview
In this project, I built a Recurrent Neural Network to generate my own [Seinfeld](https://en.wikipedia.org/wiki/Seinfeld) TV scripts. The architecture uses 200 dimensions embedding layers at first, 2 stacked LSTM layers with 256 dimensions hidden state each, and a fully connected layer in the end. After model was trained, I used it to predict a new, "fake" TV script, based on patterns it recognized in this training data.

One main problem in this project is the hyper-parameters tuning. Because the dialogues are short, it is better to use a small sequence length. Also, if you are using a small dimension of embedding layers, do not use a high dropout probability like 0.5, because these word2vec contains valuable informations of the relationship between data.

# Data
The data for this project is located [here](./data/Seinfeld_Scripts.txt), which has been crawled from the http://www.seinology.com/ website. I used part of the Seinfeld dataset of scripts from 9 seasons.

# Environment
Python: 3.6

PyTorch: 0.4.0

GPU: NVIDIA GeForce GTX 970M

Windows: 8.1

# Example Generated Script

```
jerry: well, i can't get this. i was thinking of a little problem.

jerry: oh, yeah, yeah.

kramer: well, i'm not going to be a little adjustment.

jerry: oh, yeah, i can't get this.

george: oh, no, no, no, no no no, no. no... i was thinking of that lady.

george: what do you mean?

hoyt: i don't want to get the money for you?

jerry: yeah.

jerry: you know what the hell is that?

hoyt: i don't know.

...

```

# Deliverable
Check the [**dlnd_tv_script_generation.ipynb**](./dlnd_tv_script_generation.ipynb) for all implementation.

Check the 5 example generated script in [example](./example) folder.

The [**helper.py**](./helper.py) has functions for model saving and loading.

The [**problem_unittests.py**](./problem_unittests.py) has unit tests for functions.
