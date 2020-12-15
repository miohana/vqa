# Visual Question Answering
## Repository for the discipline MO434 , from [Campinas State University](https://www.unicamp.br/unicamp/english)

## Table of Content
- [Introduction](#introduction)
- [Demo](#demo)
- [Model Overview](#model-overview)
- [Technical Aspect](#technical-aspect)
- [Running the app locally](#running-the-app-locally)
- [Project Directory Tree](#project-directory-tree)
- [Technologies Used](#technologies-used)
- [To Do](#to-do)
- [License](#license)
- [References](#references)

## Introduction
A simple Flask app to generate answer given an image and a natural language question about the image. The app uses a deep learning model, trained with Tensorflow, behind the scenes.

## Demo 
TO-DO

## Model Overview
Recent developments in Deep Learning has paved the way to accomplish tasks involving multimodal learning. Visual Question Answering (VQA) is one such challenge which requires high-level scene interpretation from images combined with language modelling of relevant Q&A. Given an image and a natural language question about the image, the task is to provide an accurate natural language answer. This is a Keras implementation of one such end-to-end system to accomplish the task.

The model architecture is based on the paper [Hierarchical Question-Image Co-Attention for Visual Question Answering](https://arxiv.org/pdf/1606.00061).

## Technical Aspect
The model used in the app is trained on [VQA 2.0](https://visualqa.org/download.html) dataset. The accuracy of the paper on this dataset is 54%. The model used in the [VQA-Flask-App](https://github.com/arya46/VQA-Flask-App) has an accuracy of 49.20%.

## Baseline
[here](https://www.overleaf.com/project/5fd6d2775c7c41162b56e40f)

## Running the app locally
*The Code is written in Python 3.7. If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip.*

First, clone this project to your local machine:
```
git clone https://github.com/miohana/unicamp-mo434.git

# change the working directory
cd unicamp-mo434
```
Then install the required packages and libraries. Run the following command:
```
pip install -r requirements.txt
```
Everything is set now. Use the following command to launch the app:
```
python main.py
```
The app will run on `http://localhost:8080/` in the browser.

## Project Directory Tree
```
├── models 
│   ├── arch.py   #contains the model final model architecture
│   └── layers.py #contains the custom layers
├── pickles 
│   ├── complete_model.h5  #the trained Keras model
│   ├── labelencoder.pkl   #LabelEncoder object
│   └── text_tokenizer.pkl #Keras tokenizer object
├── static
├── templates 
│   ├── index.html
│   └── error.html 
├── utils 
│   ├── helper_functions.py
│   └── load_pickles.py
├── LICENSE
├── README.md
├── main.py
└── requirements.txt
```
## Technologies Used
- Programming Language: Python
- ML Tools/Libraries: Keras, Tensorflow, Scikit Learn, Numpy, Pandas
- Web Tools/Libraries: Flask, HTML

## To Do
- [X] Local deployement
- [X] Explicação do problema
- [X] Arquitetura
- [X] Baseline obtido
- [X] Próximos passos
- [X] Explicação do problema
- [X] README.md update


## License
[LICENSE](https://github.com/miohana/unicamp-mo434/blob/main/LICENSE)

## References

### Main: 

Hierarchical Question-Image Co-Attention
for Visual Question Answering:
https://arxiv.org/pdf/1606.00061.pdf

Visual Question Answering with Deep Learning:
https://towardsdatascience.com/visual-question-answering-with-deep-learning-2e5e7cbfdcd4

https://github.com/arya46/VQA-Flask-App

https://github.com/arya46/portfolio_notebooks/tree/master/Visual%20Question%20Answering

### Others

https://github.com/chingyaoc/VQA-tensorflow

https://github.com/paarthneekhara/neural-vqa-tensorflow

https://towardsdatascience.com/deep-learning-and-visual-question-answering-c8c8093941bc

https://github.com/GT-Vision-Lab/VQA

https://github.com/jnhwkim/ban-vqa

https://github.com/chingyaoc/awesome-vqa

https://github.com/Cyanogenoid/pytorch-vqa

https://github.com/zhoubolei/VQAbaseline/blob/master/opensource_base.lua

Simple Baseline for Visual Question Answering: https://arxiv.org/pdf/1512.02167.pdf

Are You Talking to a Machine?
Dataset and Methods for Multilingual Image Question Answering: https://arxiv.org/pdf/1505.05612.pdf
