# Chatbot using TensorFlow 

The example on how to implement simple chatbot using seq2seq model in the python using tensorflow 1.4 version. This Chatbot example shows
the attention mechanism and bucketing as well.

## Dataset

I've used the Cornell Movie Dialogs corpuse for this example. You can download it: [here](https://www.cs.cornell.edu/~cristian/Cornell_Movie-Dialogs_Corpus.html) 

## Install

### &nbsp;&nbsp;&nbsp; Supported Python version
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Python version used in this project: 3.5+

### &nbsp;&nbsp;&nbsp; Libraries used

> *  [Pandas](http://pandas.pydata.org) 0.18.0
> *  [Numpy](http://www.numpy.org) 1.10.4
> *  [TensorFlow](https://www.tensorflow.org) 1.4.0

## Code

The core seq2seq model functions are all insude **model_utils.py**.

Data preprocessing and NLP functions are inside **cornell_data_utils.py**.

If you want to play with models hyperparameters use **config.py**.

## Run

To run this project you will need some software, like Anaconda, which provides support for running .ipynb files (Jupyter Notebook).

After making sure you have that, you can run from a terminal or cmd next lines:

`ipython notebook chatbot.ipynb`

or

`jupyter notebook chatbot.ipynb`



