# LSTM - Long Short Term Memory

---------------------------------------
## 09|02|2023

---------------------------------------

Gostaria de te passar uma quest para ser feita até o início das aulas:

Treinar a LSTM utilizando os dados do arquivo 'petr4_treinamento.csv' e avaliar o desempenho da rede com o 'petr4_teste.csv'.

Esses arquivos têm 7 colunas, ou seja, 7 atributos/features. A primeira coluna, por motivos óbvios a gente só utiliza para saber qual a amostra estamos trabalhando, já que não faz sentido prever a data. Os dados em si representam os valores da ação da Petrobrás ao longo dos dias. Como esses dados descrevem uma série temporal, nada mais justo do que utilizar a LSTM...

Primeiramente, você pode trabalhar com apenas um atributo, como, por exemplo, 'Open' (segunda coluna). A ideia é utilizar os dados dessa coluna para treinar a LSTM para que ela possa indicar qual será o valor da ação no dia seguinte.

Quando trabalhamos com séries temporais, é normal utilizarmos janelas deslizantes. Nesse caso, escolhemos X amostras sequenciais como entrada para prever o valor da amostra seguinte. Por exemplo, se definirmos o valor de X como 5, utilizaríamos as amostras de 1 a 5 para prever o valor da 6ª. Na rodada seguinte, utilizaríamos o valor das amostras de 2 a 6 para prever o valor da 7ª, e assim em diante.

Na hora de avaliar a previsão, quando for trabalhar com o arquivo de teste, você pode utilizar várias métricas: erro absoluto entre o valor real (do arquivo) e o que foi previsto pela rede, Normalized mean square error (NMSE), Root Mean Squared Error (RMSE) ou qualquer outra que julgar necessária. Para calcular essas métricas, você vai precisar de uma matriz que indique para cada amostra do arquivo de teste qual era o valor esperado e o que foi retornado pela rede. O erro absoluto, NMSE e RMSE é um valor único que indica o quanto o seu modelo errou.

A grande 'dificuldade' dessa atividade é encontrar o valor de X que vai nos retornar a melhor previsão, ou seja, o menor erro. Dessa forma, você pode plotar um gráfico em que o eixo x pode ser os valores de X que você utilizou e em y são representados os valores de uma daquelas métricas citadas anteriormente.



Acho que é isso =)

Qualquer dúvida, é só me dar um toque.

Bom resto de férias.
