# Projeto_Final_-machine_learning
## Este repositório contém a análise das viagens transatlânticas de escravizados e o uso de machine learning para prever mortes e o sucesso das viagens.

Para visualizar o notebook com mapas interativos, clique no link abaixo:

https://nbviewer.org/github/juorioli/Machine_Learning_Julia_Orioli_Project/blob/main/Projeto%20%20Final-JuliaOrioli.ipynb

# Análise de Viagens Transatlânticas de Escravizados e Modelagem Preditiva

## Descrição do Projeto
Este projeto busca explorar e prever aspectos das viagens transatlânticas de navios negreiros (tumbeiros) utilizando técnicas de Machine Learning. O objetivo principal é entender a distribuição do número de escravizados por século, ano e localidade, além de prever a probabilidade de mortes durante as viagens e se o navio chegou ao destino final.

O projeto também utiliza modelos preditivos para estimar:

O número de mortes de escravizados ao longo da viagem.
Se o navio concluiu sua viagem.
## Dataset
O dataset foi retirado do projeto Slave Voyages, que documenta mais de 36.000 viagens transatlânticas de navios negreiros realizadas entre os séculos 16 e 19 (1525 a 1864). O Codebook fornecido pela plataforma Slave Voyages detalha todas as variáveis incluídas no dataset, como:

Ano da viagem
País de origem da embarcação
Local de embarque e desembarque dos escravizados
Número de escravizados embarcados e desembarcados
Número de mortes durante a viagem
Conclusão da viagem (se o navio chegou ao destino)
Tipo de embarcação e proprietário do navio
Essas viagens eram extremamente perigosas, levando à morte de muitos escravizados, e por isso os navios foram chamados de "tumbeiros", devido ao alto número de fatalidades e à perspectiva de morte ao cruzar o Atlântico. Para os africanos, a travessia do Atlântico era conhecida como o "caminho da morte".

## Fonte dos Dados
Os dados podem ser encontrados no projeto Slave Voyages, uma plataforma aberta de pesquisa sobre a história do tráfico transatlântico de escravizados.

## Objetivos do Projeto
Análise Exploratória de Dados (EDA):

Quantificar o número de escravizados ao longo dos séculos e identificar padrões temporais e geográficos.
Explorar a mortalidade durante as viagens e investigar os fatores que contribuíram para o número de mortes.
Determinar as taxas de sucesso das viagens (se o navio chegou ao destino).
Modelos Preditivos:

Prever o número de mortes de escravizados durante as viagens utilizando diferentes algoritmos de Machine Learning.
Prever se o navio completou sua viagem com base nas variáveis fornecidas no dataset.
Ferramentas e Bibliotecas Utilizadas
##O projeto foi desenvolvido em Python e utilizou as seguintes bibliotecas:

Manipulação e análise de dados: pandas, numpy
Visualização de dados: matplotlib, seaborn, plotly, mplcursors
Modelagem e Machine Learning:
scikit-learn: Árvores de Decisão, Florestas Aleatórias, SVM, Regressão Linear, Redes Neurais (MLP)
tensorflow, keras_tuner: Para construção de redes neurais e ajuste de hiperparâmetros
Visualização de mapas: folium
Avaliação dos modelos: accuracy_score, confusion_matrix, classification_report, mean_squared_error, r2_score
## Modelos de Machine Learning
Diferentes algoritmos foram utilizados para modelagem preditiva, tanto para classificação (prever se o navio completou a viagem) quanto para regressão (prever o número de mortes):

Árvores de Decisão (DecisionTreeClassifier)
Florestas Aleatórias (RandomForestClassifier, RandomForestRegressor)
Máquinas de Vetores de Suporte (SVM)
Regressão Linear (LinearRegression)
Redes Neurais (MLPClassifier, tensorflow.keras.models.Sequential)
O ajuste de hiperparâmetros foi realizado com o auxílio do Keras Tuner e utilizando estratégias como Random Search.

# Instalação
## Pré-requisitos
Certifique-se de ter Python 3.6+ e pip instalado.
