# Classificação da Qualidade de Vinhos com Machine Learning

Projeto desenvolvido para o Tech Challenge da Fase 2 da Pós-Tech em Data Analytics.

## Objetivo

O objetivo deste projeto é desenvolver e avaliar modelos de Machine Learning capazes de prever a qualidade de vinhos a partir de suas características físico-químicas.

A variável original `quality` foi transformada em um problema de classificação binária:

- Baixa/Média Qualidade: nota menor que 7
- Alta Qualidade: nota maior ou igual a 7

O projeto busca comparar diferentes abordagens de classificação e identificar quais características possuem maior influência na previsão da qualidade dos vinhos.

## Dataset

O projeto utiliza o dataset `WineQT.csv`, composto por 1.143 amostras e características físico-químicas dos vinhos.

As variáveis utilizadas para treinamento dos modelos são:

- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol

## Modelos Utilizados

Foram utilizados dois modelos de classificação:

### Regressão Logística

Modelo linear utilizado como uma abordagem interpretável para classificação binária. As variáveis foram padronizadas utilizando `StandardScaler`.

### Random Forest

Modelo baseado em múltiplas árvores de decisão, capaz de capturar relações não lineares entre as características físico-químicas dos vinhos.

Devido ao desbalanceamento da variável alvo, os modelos foram configurados utilizando balanceamento de pesos das classes.

## Métricas de Avaliação

Os modelos foram avaliados utilizando:

- Acurácia
- Precisão
- Recall
- F1-Score
- ROC-AUC
- Matriz de Confusão

A utilização de diferentes métricas é importante devido ao desbalanceamento das classes do conjunto de dados.

