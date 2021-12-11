# Interactive-Chatbot
Chatbot, a conversational dialogue engine built with tensorflow, Pytorch, LSTM networks to generate responses based on collections of known conversations. The language independent design of ChatterBot allows it to be trained to speak any language.

An example of typical input would be something like this:

> **user:** Good morning! How are you doing?  
> **bot:**  I am doing very well, thank you for asking.  
> **user:** You're welcome.  
> **bot:** Do you like hats?  

## How it works

An untrained instance of ChatterBot starts off with no knowledge of how to communicate. Each time a user enters a statement, the library saves the text that they entered and the text that the statement was in response to. As ChatterBot receives more input the number of responses that it can reply and the accuracy of each response in relation to the input statement increase. The program selects the closest matching response by searching for the closest matching known statement that matches the input, it then returns the most likely response to that statement based on how frequently each response is issued by the people the bot communicates with.

# ChatBot using LSTM Networks
 Long Short Term Memory networks – usually just called “LSTMs” – are a special kind of RNN, capable of learning long-term dependencies. They were introduced by [Hochreiter & Schmidhuber (1997)](http://www.bioinf.jku.at/publications/older/2604.pdf), and were refined and popularized by many people in following work.1 They work tremendously well on a large variety of problems, and are now widely used.

LSTMs are explicitly designed to avoid the long-term dependency problem. Remembering information for long periods of time is practically their default behavior, not something they struggle to learn!

All recurrent neural networks have the form of a chain of repeating modules of neural network. In standard RNNs, this repeating module will have a very simple structure, such as a single tanh layer.

![](https://github.com/Abhishek-Aditya-bs/StockPrice-Prediction-Using-Pytorch-Neural-Network/blob/main/LSTM-pic.png)

<p align='center'> The repeating module in a standard RNN contains a single layer.</p>

LSTMs also have this chain like structure, but the repeating module has a different structure. Instead of having a single neural network layer, there are four, interacting in a very special way.

![](https://github.com/Abhishek-Aditya-bs/StockPrice-Prediction-Using-Pytorch-Neural-Network/blob/main/LSTM-chain.png)

<p align='center'> The repeating module in an LSTM contains four interacting layers.</p>

![](https://github.com/Abhishek-Aditya-bs/StockPrice-Prediction-Using-Pytorch-Neural-Network/blob/main/LSTM-notation.png)

In the above diagram, each line carries an entire vector, from the output of one node to the inputs of others. The pink circles represent pointwise operations, like vector addition, while the yellow boxes are learned neural network layers. Lines merging denote concatenation, while a line forking denote its content being copied and the copies going to different locations.

# ChatBot using Pytorch
<p align='Center'><img src="https://github.com/Abhishek-Aditya-bs/Interactive-Chatbot/blob/main/ChatBot%20-%20PyTorch/logo.png" /> </p>

Details on Implementation can be found [here](https://github.com/Abhishek-Aditya-bs/Interactive-Chatbot/blob/main/ChatBot%20-%20PyTorch/chatbot.py)

Clone the [Repository](https://github.com/Abhishek-Aditya-bs/Interactive-Chatbot/tree/main/ChatBot%20-%20PyTorch) and install the necessary dependecies :

1. numpy
2. pandas
3. re
4. torch 
5. torchvision

Run `python3 chatbot.py` in terminal to get the ChatBot up and running.

# ChatBot using Tensorflow 
<p align='Center'><img src="https://github.com/Abhishek-Aditya-bs/Interactive-Chatbot/blob/main/ChatBot%20-%20TensorFlow/tf_logo.png" /> </p>

The [Repository](https://github.com/Abhishek-Aditya-bs/Interactive-Chatbot/tree/main/ChatBot%20-%20TensorFlow) shows how to implement simple chatbot using seq2seq model in the python using tensorflow. This Chatbot example shows
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




