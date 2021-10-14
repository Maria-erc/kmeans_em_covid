# kmeans_em_covid
Algoritmo K-means para classificação de sintomas

## Objetivo
O objetivo desse código foi classificar sintomas em 4 categorias: covid, resfriado, gripe e rinite. Para isso, utilizou-se o algoritmo de classificação K-Means.

## Dados

O banco de dados é composto por 5 colunas: febre, fadiga, mal-estar, dor de garganta e diagnóstico, além de possuir 80 instâncias.

Esses sintomas são figurativos, mas possuem certa aproximação com a realidade. Cada sintoma possui um número, que é a classificação da intensidade do sintoma em uma escala de 0 a 10. Assim, com base nesses números desses 4 sintomas foi determinado o diagnóstico. Para a criação desses números fictícios teve-se um estudo aprofundado dos sintomas e da intensidade dos sintomas de cada uma dessas doenças.


Por exemplo: febre 6,5; fadiga 5; mal-estar 9; dor de garganta 0. Observando esses números, analisa-se que são características muito mais comuns ao vírus covid 19 do que nas outras 3 doenças, logo rotulou-se essa instância como com diagnóstivo de covid. Assim foi feito em cada uma das isntâncias, até formar todo o dataframe que foi usado de treinamento para o modelo K-means.

## Resultado
O modelo K-means conseguiu fazer uma classificação satisfatória das instâncias de treinamento. Pode-se dizer que as classes do modelo 0, 1, 2 e 3 fazem referência aos respectivos diagnósticos: rinite, gripe, covid e resfriado.
