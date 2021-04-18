# Mask Classifier (Classificação automática de rostos com ou sem máscara usando DNNs e um dataset artificial)

## Índice
* [Conteúdos](#conteúdos)
* [Informações Gerais](#informações-gerais)
* [Tecnologias utilizadas](#tecnologias-utilizadas)
* [Instalação do Environment](#instalação-do-environment)
* [Conjunto de dados](#conjunto-de-dados)
* [Aplicativo Android](#aplicativo-android)
* [Artigo](#artigo)


## Conteúdos

O presente repositório é composto por 5 Jupyter Notebooks: 
* [draw_mask](https://github.com/mask-classifier/mask-classifier/blob/main/draw_mask.ipynb)
* [image_reduce](https://github.com/mask-classifier/mask-classifier/blob/main/image_reduce.ipynb)
* [treino_e_teste](https://github.com/mask-classifier/mask-classifier/blob/main/treino_e_teste.ipynb)
* [validacao](https://github.com/mask-classifier/mask-classifier/blob/main/validacao.ipynb)
* [camera](https://github.com/mask-classifier/mask-classifier/blob/main/camera.ipynb)


## Informações Gerais

Com os conteúdos do presente repositório, cria-se um conjunto de dados dividido entre fotos de rostos humanos e fotos de rostos humanos utilizando máscaras artificialmente geradas, treina-se e testa-se um modelo classificador utilizando Redes Neurais Profundas (Deep Neural Networks), valida-se o modelo classificador utilizando fotos reais de pessoas utilizando ou não máscaras faciais e, por fim, valida-se o modelo utilizando a webcam do computador em tempo real.


## Tecnologias utilizadas
* Python 3.6.12
* dlib 19.7.0
* imutils 0.5.4
* Keras 2.4.3
* Keras-Applications 1.0.4
* Keras-Preprocessing 1.1.0
* matplotlib 3.3.4
* mlxtend 0.18.0
* numpy 1.18.1
* pandas 1.1.5
* Pillow 8.2.0
* scikit-image 0.17.2
* scikit-learn 0.24.1
* seaborn 0.11.1
* sklearn 0.0
* tensorflow 2.2.2


## Instalação do Environment

Primeiro, você deve baixar e instalar o [Anaconda](https://www.anaconda.com/products/individual#Downloads).

Após a instalação, baixe o arquivo do environment [mask-classifier.yml](https://github.com/mask-classifier/mask-classifier/blob/main/environment/mask-classifier.yml).

Então, abra o Anaconda Prompt e navegue até a pasta onde o arquivo mask-classifier.yml foi baixado. Por exemplo, no caso de ser a pasta padrão de downloads, digite: ```cd Downloads```.

Por fim, para criar o environment, digite ```conda env create -f mask-classifier.yml```.


## Conjunto de dados
O dataset criado contém 10.000 imagens com tamanho de 224x224 e em 50% delas foram geradas máscaras artificiais.   
Se for utilizar da forma como está disposto nas pastas do respositório, descompacte o conjunto de dados dentro da pasta ```dataset/```.

Link para o conjunto de dados no Google Drive: https://drive.google.com/file/d/1Fx2Qzziri0y5YHr4p49uu6xCEc-s0uUO/view?usp=sharing

Exemplo de rostos com máscara gerados:   
![Pessoa com máscara artificial](https://i.imgur.com/MU5PWpZ.jpg) ![Pessoa com máscara artificial](https://i.imgur.com/WmI1acY.jpg)

O dataset utilizado foi coletado pela Nvidia e consiste de 70.000 fotos de rostos de pessoas retiradas do Flickr.   

Link para o dataset completo no Kaggle: https://www.kaggle.com/xhlulu/flickrfaceshq-dataset-nvidia-resized-256px   

Caso pretenda re-criar o dataset usado com uma quantidade maior, menor ou com alguma configuração diferente, descompacte dentro da pasta ```dataset/```, use o código do [image_reduce](https://github.com/mask-classifier/mask-classifier/blob/main/image_reduce.ipynb) para reduzir as imagens e depois use o código do [draw_mask](https://github.com/mask-classifier/mask-classifier/blob/main/draw_mask.ipynb) para gerar as máscaras.   
## Aplicativo Android:
Foi desenvolvido um aplicativo Android que permite demonstrar a utilização do modelo classificador em uma aplicação em tempo real.

Link para download do aplicativo .apk:
https://drive.google.com/file/d/1Tw9jWWdX_jBY90cl591qGXtFJ8j6bM-d/view?usp=sharing


## Artigo:

#### Resumo:  

A pandemia de COVID-19 tem sido um problema significativo para a saúde da população de todo o mundo. De acordo com a Organização Mundial da Saúde, a propagação do vírus ocorre através de gotículas geradas quando as pessoas respiram, falam, tossem ou espirram. Portanto, utilizar máscaras de proteção individual mostrou-se eficiente para reduzir a propagação do vírus em espaços coletivos. Neste contexto, observa-se a necessidade de sistemas de detecção de uso de máscara para monitoramento das medidas preventivas e sanitárias. Uma solução possível é utilizar redes neurais de aprendizagem profunda para desenvolver algoritmos de detecção automática que solucionem este problema. Algumas destas redes podem ser embarcadas para execução em tempo real em sistemas com baixa capacidade computacional, operando até mesmo em smartphones. Para identificar rostos com máscaras, é necessário criar um modelo classificador, um processo que necessita de dados rotulados para o treinamento supervisionado. Apesar disso, devido à baixa disponibilidade desses dados para esta tarefa, propusemos neste trabalho a criação de um conjunto vasto de dados artificiais simulando rostos com máscaras e tornando assim a tarefa de treinamento do modelo possível.

Link para o artigo completo:
https://drive.google.com/file/d/1kWfwqp3Ae0H5Owy1ctnEyaO54w97cyEi/view?usp=sharing


# Mask Classifier (Automatic classification of faces with or without face masks using DNNs and an artificial dataset)

## Table of contents
* [Contents](#contents)
* [General information](#general-information)
* [Technologies](#technologies)
* [Environment installation](#environment-installation)
* [Dataset](#dataset)
* [Android application](#android-application)
* [Paper](#paper)


## Contents

This repository is composed of 5 Jupyter Notebooks: 
* [draw_mask](https://github.com/mask-classifier/mask-classifier/blob/main/draw_mask.ipynb)
* [image_reduce](https://github.com/mask-classifier/mask-classifier/blob/main/image_reduce.ipynb)
* [treino_e_teste](https://github.com/mask-classifier/mask-classifier/blob/main/treino_e_teste.ipynb)
* [validacao](https://github.com/mask-classifier/mask-classifier/blob/main/validacao.ipynb)
* [camera](https://github.com/mask-classifier/mask-classifier/blob/main/camera.ipynb)


## General information

With the content of this repository, a dataset composed of photos of human faces and photos of human faces wearing artificially generated face masks is made, a classifier model made using Deep Neural Networks is trained and tested, the model is validated using a dataset of photos of people wearing real face masks or not, and, finally, the model is validated in real time using a webcam.

## Technologies
* Python 3.6.12
* dlib 19.7.0
* imutils 0.5.4
* Keras 2.4.3
* Keras-Applications 1.0.4
* Keras-Preprocessing 1.1.0
* matplotlib 3.3.4
* mlxtend 0.18.0
* numpy 1.18.1
* pandas 1.1.5
* Pillow 8.2.0
* scikit-image 0.17.2
* scikit-learn 0.24.1
* seaborn 0.11.1
* sklearn 0.0
* tensorflow 2.2.2


## Environment installation

First, you must download and install [Anaconda](https://www.anaconda.com/products/individual#Downloads).

After the installation, download the environment file [mask-classifier.yml](https://github.com/mask-classifier/mask-classifier/blob/main/environment/mask-classifier.yml).

Then, open Anaconda Prompt and navigate to the folder where the mask-classifier.yml file was downloaded. For example, in case of the default downloads folder, simply write ```cd Downloads```.

Finally, to create the environment, type ```conda env create -f mask-classifier.yml```.


## Dataset
The dataset we created has 10.000 images with size 224x224 and 50% of those have artificially generated face masks.
If you want to use it in the same way it's disposed on the repository, unzip the dataset inside the ```dataset/``` folder.  

Link for the dataset in Google Drive: https://drive.google.com/file/d/1Fx2Qzziri0y5YHr4p49uu6xCEc-s0uUO/view?usp=sharing   
Examples of faces with artificially generated face masks:   
![Person Wearing an artificially generated face mask](https://i.imgur.com/MU5PWpZ.jpg) ![Person Wearing an artificially generated face mask](https://i.imgur.com/WmI1acY.jpg)

The original dataset we used was collected by Nvidia and consists of 70.000 photos of human faces taken from Flickr.   
Link for the complete dataset on Kaggle: https://www.kaggle.com/xhlulu/flickrfaceshq-dataset-nvidia-resized-256px   

In case you intend to recreate the dataset with a bigger or smaller amount, or with any different configuration, unzip it inside the ```dataset/``` folder, use the [image_reduce](https://github.com/mask-classifier/mask-classifier/blob/main/image_reduce.ipynb) code to reduce the images and then use the [draw_mask](https://github.com/mask-classifier/mask-classifier/blob/main/draw_mask.ipynb) code to generate the artificial face masks.

## Android application:
An Android app was developed in order to demonstrate the utilization of the classifier model in a real time application.

Link to download the .apk file:
https://drive.google.com/file/d/1Tw9jWWdX_jBY90cl591qGXtFJ8j6bM-d/view?usp=sharing


## Paper:

#### Abstract:  

The COVID-19 pandemic has been a significant public health problem around the world. According to the World Health Organization, the contamination by the virus happens through droplets spread when people breathe, speak, cough or sneeze. Therefore, using face masks has shown to be an efficient way to reduce virus propagation in collective spaces. In this context, the need for a face mask detection system as a way of enforcing and monitoring preventive and sanitary measures is urgent. With Deep Learning Neural Networks (DNNs), it is possible to develop algorithms for automatic detection that solve this problem, and also do not require powerful hardware to run, and can run in real time embedded in systems as computationally powerful as common smartphones. To train a supervised learning model, data with appropriate labels is needed. Despite that, because there was not a way of gathering enough data to complete this task, a Simulated Masked Face Dataset (SMFD) is proposed in this work.


Link for the full paper (in portuguese):
https://drive.google.com/file/d/1kWfwqp3Ae0H5Owy1ctnEyaO54w97cyEi/view?usp=sharing
