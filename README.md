# unicamp-mo434 - Visual Question Answering

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

## Introduction
A simple Flask app to generate answer given an image and a natural language question about the image. The app uses a deep learning model, trained with Tensorflow, behind the scenes.

## Demo 
TO-DO

## Model Overview
Recent developments in Deep Learning has paved the way to accomplish tasks involving multimodal learning. Visual Question Answering (VQA) is one such challenge which requires high-level scene interpretation from images combined with language modelling of relevant Q&A. Given an image and a natural language question about the image, the task is to provide an accurate natural language answer. This is a Keras implementation of one such end-to-end system to accomplish the task.

The model architecture is based on the paper [Hierarchical Question-Image Co-Attention for Visual Question Answering](https://arxiv.org/pdf/1606.00061).

## Technical Aspect
The model used in the app is trained on [VQA 2.0](https://visualqa.org/download.html) dataset. The accuracy of the paper on this dataset is 54%. The model used in the Flask app has an accuracy of 49.20%.

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
- [ ] Explicação do problema
- [ ] Arquitetura
- [ ] Baseline obtido
- [ ] Próximos passos
- [ ] Explicação do problema
- [ ] Atualização README.md


## License
[LICENSE](https://github.com/miohana/unicamp-mo434/blob/main/LICENSE)