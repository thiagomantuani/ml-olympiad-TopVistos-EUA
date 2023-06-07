# ML Olympiad for Students - TopVistos EUA (Kaggle) - 7º Lugar

Solução:
  1. Colocar os dados na pasta data. (os dados podem ser obtidos em https://www.kaggle.com/competitions/ml-olympiad-for-students-topvistos-eua)
  2. Rodar o solution.ipynb
 
A solução proposta é um stacking ensemble que utiliza quatro modelos base: Random Forest, XGBoost, CatBoost e LightGBM. Para a etapa de predição final, é utilizado um meta-classificador Logistic Regression. Além disso, uma média ponderada entre os modelos Random Forest e Logistic Regression é calculada, juntamente com as médias das previsões dos outros modelos, para aumentar a precisão da previsão final.
Para determinar se um exemplo pertence à classe "Aprovado" ou "Negado", foi definido um limiar com base nos 67% principais exemplos, levando em consideração a porcentagem de exemplos positivos na amostra de treinamento. Essa abordagem permite que o modelo faça previsões mais confiáveis, aumentando sua capacidade de generalização.
