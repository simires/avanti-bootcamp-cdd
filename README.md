# Análise e Predição de Sobreviventes do Titanic

Projeto de ciência de dados para investigar padrões de sobrevivência dos passageiros do Titanic, com base na base de dados Titanic - Machine Learning from Disaster. Inclui análise exploratória dos dados e comparação de quatro algoritmos de classificação — KNN, Árvore de Decisão, Regressão Logística e Naive Bayes — com validação cruzada K-Fold e otimização de hiperparâmetros via GridSearchCV. Este projeto foi desenvolvido como atividade do Bootcamp de Ciência de Dados da Escola Atlântico Avanti do [Instituto Atlântico](https://www.atlantico.com.br/).

## Objetivos
 - Compreender o perfil dos passageiros do Titanic por meio de análise exploratória dos dados
 - Investigar a relação entre variáveis como classe social, sexo, idade e tarifa paga com a sobrevivência
 - Identificar e tratar dados faltantes e preparar os dados para modelagem
 - Treinar e comparar quatro modelos de classificação para prever a sobrevivência dos passageiros
 - Avaliar o desempenho dos modelos com métricas de acurácia, precisão, recall e F1-score

## Notebooks
Os notebooks estão localizados no diretório ``notebooks/`` e contêm as seguintes documentações:
| **Notebook** | **Descrição** |
| :------- | :------ |
| [00-download_data.ipynb](https://github.com/simires/avanti-bootcamp-cdd/blob/master/notebooks/00-download_data.ipynb) | Obtenção dos dados e construção do dicionário de dados. |
| [01-exploratory_data_analysis.ipynb](https://github.com/simires/avanti-bootcamp-cdd/blob/master/notebooks/01-exploratory_data_analysis.ipynb) | Análise exploratória dos dados: estatísticas descritivas, distribuições, dados faltantes e investigação de padrões de sobrevivência por meio de visualizações. |
| [02-comparative-analysis.ipynb](https://github.com/simires/avanti-bootcamp-cdd/blob/master/notebooks/02-comparative-analysis.ipynb) | Pré-processamento com pipelines do scikit-learn e comparação de modelos de classificação avaliados por acurácia, precisão, recall e F1-score. |   

## Resultados

### Análise exploratória
- A maioria dos passageiros não sobreviveu, era do sexo masculino e viajava na terceira classe
- Passageiros que pagaram tarifas mais altas — predominantemente da primeira classe — tiveram maiores chances de sobrevivência
- Mulheres de até aproximadamente 40 anos apresentaram maior taxa de sobrevivência em comparação aos homens da mesma faixa etária
- Homens com maiores chances de sobreviver eram em geral mais jovens do que as mulheres sobreviventes
- Passageiros da terceira classe eram em média mais jovens do que os das classes superiores

### Comparação de modelos de classificação
- O modelo K-Nearest Neighbors obteve os resultados mais confiáveis nos testes de acurácia, precisão, recall e F1-score.
