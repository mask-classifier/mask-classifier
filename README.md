# Mask Classifier (Classificação automática de rostos com ou sem máscara usando DNNs e um dataset artificial)

# Tabela de conteúdos
* [Informações Gerais](#informações-gerais)
* [Tecnologias utilizadas](#tecnologias-utilizadas)
* [Instalação do Environment](#instalação-do-environment)
* [Dataset](#dataset)
* [Aplicativo Android](#aplicativo-android)
* [Artigo](#artigo)

# Informações Gerais
O presente repositório contém 5 Jupyter Notebooks.

# Tecnologias utilizadas
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

# Instalação do Environment

Primeiro, você deve baixar o Anaconda pelo link: https://www.anaconda.com/products/individual#Downloads.

Após instalar o Anaconda, baixe este [arquivo](/environments/mask-classifier.yml).

Com o arquivo, abra o Anaconda Prompt (pesquise na barra de pesquisa do windows) vá até sua pasta onde o arquivo mask-classifier.yml foi baixado, no caso de ser a pasta de downloads, para isso digite: ```cd Downloads```.

Por fim, para criar o environment, digite ```conda env create -f mask-classifier.yml```.

# Dataset

O dataset utilizado foi coletado pela Nvidia e consiste de 70.000 fotos de rostos de pessoas retiradas do Flickr.

Link para o dataset no Kaggle:
https://www.kaggle.com/xhlulu/flickrfaceshq-dataset-nvidia-resized-256px

# Aplicativo Android:
Foi desenvolvido um aplicativo Android que permite demonstrar a utilização do modelo classificador em uma aplicação em tempo real.

Link para download do aplicativo .apk:
https://drive.google.com/file/d/1Tw9jWWdX_jBY90cl591qGXtFJ8j6bM-d/view?usp=sharing

# Artigo:

### Resumo:  

A pandemia de COVID-19 tem sido um problema significativo para a saúde da população de todo o mundo. De acordo com a Organização Mundial da Saúde, a propagação do vírus ocorre através de gotículas geradas quando as pessoas respiram, falam, tossem ou espirram. Portanto, utilizar máscaras de proteção individual mostrou-se eficiente para reduzir a propagação do vírus em espaços coletivos. Neste contexto, observa-se a necessidade de sistemas de detecção de uso de máscara para monitoramento das medidas preventivas e sanitárias. Uma solução possível é utilizar redes neurais de aprendizagem profunda para desenvolver algoritmos de detecção automática que solucionem este problema. Algumas destas redes podem ser embarcadas para execução em tempo real em sistemas com baixa capacidade computacional, operando até mesmo em smartphones. Para identificar rostos com máscaras, é necessário criar um modelo classificador, um processo que necessita de dados rotulados para o treinamento supervisionado. Apesar disso, devido à baixa disponibilidade desses dados para esta tarefa, propusemos neste trabalho a criação de um conjunto vasto de dados artificiais simulando rostos com máscaras e tornando assim a tarefa de treinamento do modelo possível.

Link para o artigo completo:
https://drive.google.com/file/d/1kWfwqp3Ae0H5Owy1ctnEyaO54w97cyEi/view?usp=sharing
