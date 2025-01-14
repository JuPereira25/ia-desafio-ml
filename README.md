# ia-desafio-ml
Previsão de Vendas de uma Loja
Este projeto tem como objetivo prever as vendas de uma loja para o mês de dezembro, com base em dados históricos mensais de vendas. Utilizei técnicas de regressão 
linear para modelar a relação entre o mês e as vendas, utilizando o conjunto de dados fornecidos. Abaixo, explico os principais passos seguidos para alcançar a 
previsão e a análise dos dados.

Etapas Realizadas:
 1. Tratamento de Dados(EDA):

    - O conjunto de dados foi carregado em um DataFrame usando uma biblioteca pandas, com informações sobre os meses do ano e as vendas correspondentes a cada mês.
    - Os dados foram analisados ​​utilizando métodos como info()e dtypes para verificar a estrutura e tipos de dados.
    - O mês foi convertido de uma string para um valor numérico ( mes_numero), para facilitar o treinamento do modelo de regressão.

 2. Formatação dos Dados:

    - A coluna de meses foi transformada em valores numéricos (de 1 a 12) para representar cada mês de forma sequencial.
    - A coluna de vendas foi mantida como valores inteiros, representando as vendas mensais da loja.

 3. Treinamento do Modelo:

    - Utilizamos o algoritmo de regressão linear da biblioteca scikit-learn para treinar um modelo, com base em nossos dados históricos.
    - O conjunto de dados foi dividido em dados de treino e dados de teste utilizando a função train_test_split.
    - O modelo foi treinado com a variável independente mes_numero e a variável dependente vendas.

 4. Previsão de Vendas para Dezembro:

    - Após treinar o modelo, realizamos a previsão de vendas para o mês de dezembro (mês número 12).
    - A previsão foi feita utilizando o modelo treinado e foi apresentado no formato de número arredondado para duas casas decimais.

 5. Análise Visual:

   - Histograma: Foi gerado um histograma de vendas mensais para visualizar a distribuição dos dados. Isso ajudou a entender o comportamento das vendas ao longo do 
ano.
   - Gráfico de dispersão: Foi criado um gráfico de dispersão para mostrar a relação entre os meses e as vendas. Uma linha de regressão foi traçada sobre o gráfico 
para mostrar a tendência das vendas ao longo do tempo.

Resultados:

  - O modelo de regressão linear obteve um R² Score de 0,96, indicando que o modelo é capaz de explicar 96% da variabilidade das vendas mensais.
  - O Erro Quadrático Médio (MSE) foi de 2096.18, o que sugere que a previsão está bem ajustada aos dados históricos.

Conclusão:
  - A previsão das vendas para o mês de Dezembro foi realizada com sucesso e fornece uma base para decisões comerciais. A análise visual dos dados, com histogramas 
e gráficos de dispersão, permitiu identificar tendências nas vendas ao longo do ano. Este projeto é uma demonstração simples, mas poderosa, de como usar 
regressão linear para prever séries temporais de dados, como vendas mensais de uma loja.

