# Speech Recognition model

This is a Deep Learning model that gets an audio input and predicts/writes down what it is said in the audio.
It is written in Python with Pytorch framework and it is trained in Google Colab.

## Hypothesis 

The speech recognition model output will generate better predictions if we add Attention.

## Environment: Google Colab setup

It is possible to run/train this model in Google Colab. In order to do this, you need a google account and Google Drive access. Then you have to follow the next steps:

* First of all, we need to download this audio encoder named PASE from this 	github repo: https://github.com/santi-pdp/pase

* Place PASE (the whole folder named pase-master) in a folder named "Project AI" in the root path of your Google Drive. 

* Now you have to download this file (FE_e199.ckpt) from here https://drive.google.com/file/d/1xwlZMGnEt9bGKCVcqDeNrruLFQW5zUEW/view and place it inside pase-master folder.

* The dataset can be downloaded from here: 
    * Audios dataset: https://drive.google.com/drive/folders/1oQGKrV5JCZ6EHp4k3UBtqYUreuxensB4?usp=sharing
    * Texts dataset: https://drive.google.com/drive/folders/18MuvbMBwuhl8zs4cb7h4M1o0b3tAYI7O?usp=sharing
    * It can be downloaded alternatively from here: https://groups.csail.mit.edu/sls/downloads/flickraudio/index.cgi

* Both flickr_text and flickr_audio datasets need to be placed in "Project AI" folder.

* Finally we only need to select "type of environment" -> GPU at Google Colab and run all the "Install & Import" section instructions.

## The dataset

We have used a Flickr dataset that consists of 40000 audio files and 40000 text files. In the text files you can read what it is said in the audio files. 

## Data preprocessing

In order to train the model, text dataset needs to be preprocessed. We have done the next modifications to all the sentences in order to create the dictionary:

* We have removed the capital letters
* We have removed accent marks
* We have removed punctuation marks

Before feeding our model and begin training it we have ensured that lemmatization is done to all of the sentences. 

## Experiments

### Experiment 1: Attention vs No Attention


### Experiment 2: Number of epochs


### Experiment 3: Embedding size


## Problems 


## Conclusions
