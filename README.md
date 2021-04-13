# Mask Classifier (Classificação automática de rostos com ou sem máscara usando DNNs e um dataset artificial)

## Índice
* [Conteúdos](#conteudos)
* [Informações Gerais](#informações-gerais)
* [Tecnologias utilizadas](#tecnologias-utilizadas)
* [Instalação do Environment](#instalação-do-environment)
* [Dataset](#dataset)
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
* tensorflow-estimator 2.2.0


## Instalação do Environment

Primeiro, você deve baixar e instalar o [Anaconda](https://www.anaconda.com/products/individual#Downloads).

Após a instalação, baixe [este arquivo](https://github.com/mask-classifier/mask-classifier/blob/main/environment/mask-classifier.yml).

Com o arquivo, abra o Anaconda Prompt e navegue até a pasta onde o arquivo mask-classifier.yml foi baixado. Por exemplo, no caso de ser a pasta padrão de downloads, digite: ```cd Downloads```.

Por fim, para criar o environment, digite ```conda env create -f mask-classifier.yml```.


## Dataset

O dataset utilizado foi coletado pela Nvidia e consiste de 70.000 fotos de rostos de pessoas retiradas do Flickr.

Link para o dataset no Kaggle:
https://www.kaggle.com/xhlulu/flickrfaceshq-dataset-nvidia-resized-256px

Caso prefira, você pode utilizar o dataset com 10.000 imagens que ja foi gerado.

Link para o dataset no Drive:
https://drive.google.com/file/d/1Fx2Qzziri0y5YHr4p49uu6xCEc-s0uUO/view?usp=sharing

Exemplo de rostos com máscara gerados: ![alt text](https://i.imgur.com/MU5PWpZ.jpg) ![alt text](https://i.imgur.com/WmI1acY.jpg)

## Aplicativo Android:
Foi desenvolvido um aplicativo Android que permite demonstrar a utilização do modelo classificador em uma aplicação em tempo real.

Link para download do aplicativo .apk:
https://drive.google.com/file/d/1Tw9jWWdX_jBY90cl591qGXtFJ8j6bM-d/view?usp=sharing


## Artigo:

#### Resumo:  

A pandemia de COVID-19 tem sido um problema significativo para a saúde da população de todo o mundo. De acordo com a Organização Mundial da Saúde, a propagação do vírus ocorre através de gotículas geradas quando as pessoas respiram, falam, tossem ou espirram. Portanto, utilizar máscaras de proteção individual mostrou-se eficiente para reduzir a propagação do vírus em espaços coletivos. Neste contexto, observa-se a necessidade de sistemas de detecção de uso de máscara para monitoramento das medidas preventivas e sanitárias. Uma solução possível é utilizar redes neurais de aprendizagem profunda para desenvolver algoritmos de detecção automática que solucionem este problema. Algumas destas redes podem ser embarcadas para execução em tempo real em sistemas com baixa capacidade computacional, operando até mesmo em smartphones. Para identificar rostos com máscaras, é necessário criar um modelo classificador, um processo que necessita de dados rotulados para o treinamento supervisionado. Apesar disso, devido à baixa disponibilidade desses dados para esta tarefa, propusemos neste trabalho a criação de um conjunto vasto de dados artificiais simulando rostos com máscaras e tornando assim a tarefa de treinamento do modelo possível.

Link para o artigo completo:
https://drive.google.com/file/d/1kWfwqp3Ae0H5Owy1ctnEyaO54w97cyEi/view?usp=sharing
