# kmeans_em_covid
Algoritmo K-means para classificação de sintomas

## Objetivo
O objetivo desse código foi classificar sintomas em 4 categorias: covid, resfriado, gripe e rinite. Para isso, utilizou-se o algoritmo de classificação K-Means.

## Dados

O banco de dados é composto por 5 colunas: febre, fadiga, mal-estar, dor de garganta e diagnóstico, além de possuir 80 instâncias.

Esses sintomas são figurativos, mas possuem certa aproximação com a realidade. Cada sintoma possui um número, que é a classificação da intensidade do sintoma em uma escala de 0 a 10. Assim, com base nesses números desses 4 sintomas foi determinado o diagnóstico. Para a criação desses números fictícios teve-se um estudo aprofundado dos sintomas e da intensidade dos sintomas de cada uma dessas doenças.

![image](https://user-images.githubusercontent.com/79197619/137371580-74c2a8c7-2249-41f7-be09-ab086a3c35e4.png)



Por exemplo: febre 6,5; fadiga 5; mal-estar 9; dor de garganta 0. Observando esses números, analisa-se que são características muito mais comuns ao vírus covid 19 do que nas outras 3 doenças, logo rotulou-se essa instância como com diagnóstivo de covid. Assim foi feito em cada uma das isntâncias, até formar todo o dataframe que foi usado de treinamento para o modelo K-means.

## Resultado
O modelo K-means conseguiu fazer uma classificação satisfatória das instâncias de treinamento. Pode-se dizer que as classes do modelo 0, 1, 2 e 3 fazem referência aos respectivos diagnósticos: rinite, gripe, covid e resfriado.

Nesse gráfico plotado no código, o eixo x é febre e o eixo y é fadiga. Observa-se que quanto maior febre e maior fadiga há o cluster 2, ou seja, indica que são características de sintomas mais prováveis da doença covid.

![image](https://user-images.githubusercontent.com/79197619/137368866-120866b7-411d-44bf-90c8-757f729e7cbd.png)

Outro exemplo é o gráfico abaixo, onde é possível ver que se uma pessoa está com dor de garganta moderada a forte (5 a 10 na numeração) e febre leve a moderada 
(0 a 5) há o cluster 3, ou seja, é mais provável que ela tenha uma gripe do que com as demais doenças mencionadas.

![image](https://user-images.githubusercontent.com/79197619/137370421-56d5d134-ffb0-4fb7-94fa-221891c6d7f3.png)

