# Projeto de Preços de Imóveis Utilizando Regressão Linear

## 📋 Sobre o Projeto

Este projeto tem como objetivo desenvolver um modelo preditivo para estimar preços de imóveis com base em suas características físicas. Utilizando técnicas de regressão linear, o modelo identifica os fatores mais relevantes na determinação do valor de um imóvel e quantifica a influência de cada característica no preço final.

## 🎯 Objetivos

- Estimar preços de imóveis com base em suas características
- Identificar os aspectos que mais contribuem para a precificação
- Determinar qual característica tem maior influência no preço final
- Desenvolver uma ferramenta para precificar novos imóveis

## 📊 Dados

O conjunto de dados utilizado é inspirado no dataset "House Prices" do Kaggle e contém 1438 registros de imóveis com as seguintes variáveis:

- `area_primeiro_andar`: Área em metros quadrados do primeiro andar
- `existe_segundo_andar`: Variável binária (0 ou 1) indicando a existência de segundo andar
- `area_segundo_andar`: Área em metros quadrados do segundo andar
- `quantidade_banheiros`: Número de banheiros no imóvel
- `capacidade_carros_garagem`: Capacidade da garagem em número de carros
- `qualidade_da_cozinha_Excelente`: Variável binária (0 ou 1) indicando se a cozinha é de qualidade excelente
- `preco_de_venda`: Preço de venda do imóvel (variável alvo)

## 🔍 Análise Exploratória

A análise exploratória revelou correlações importantes entre as variáveis e o preço de venda:

| Variável | Correlação com Preço |
|----------|----------------------|
| capacidade_carros_garagem | 0.64 |
| area_primeiro_andar | 0.62 |
| quantidade_banheiros | 0.56 |
| qualidade_da_cozinha_Excelente | 0.50 |
| area_segundo_andar | 0.31 |
| existe_segundo_andar | 0.14 |

A matriz de correlação completa foi visualizada através de um heatmap, confirmando que a capacidade da garagem e a área do primeiro andar são os fatores mais determinantes no preço dos imóveis.

## 🧮 Modelagem

O projeto utiliza regressão linear para modelar a relação entre as características dos imóveis e seus preços. O processo de modelagem incluiu:

1. Divisão dos dados em conjuntos de treino (70%) e teste (30%)
2. Treinamento do modelo utilizando as variáveis selecionadas
3. Avaliação do modelo através de métricas como R², erro médio absoluto e erro quadrático médio
4. Análise dos resíduos para verificar a qualidade do ajuste

## 📈 Resultados

O modelo de regressão linear apresentou bom desempenho na previsão de preços, com os seguintes insights principais:

- A capacidade da garagem é o fator mais relevante na determinação do preço
- A área do primeiro andar tem forte impacto no valor do imóvel
- A quantidade de banheiros apresenta influência significativa no preço
- Uma cozinha de qualidade excelente pode aumentar consideravelmente o valor do imóvel
- A área do segundo andar tem impacto menor que a do primeiro andar

## 🏠 Exemplo de Aplicação

Para um imóvel com as seguintes características:
- Área do primeiro andar: 100m²
- Sem segundo andar
- 2 banheiros
- Garagem para 2 carros
- Cozinha padrão (não excelente)

O modelo estima um preço de aproximadamente R$ 686.448,23.

## 🛠️ Tecnologias Utilizadas

- Python
- Pandas para manipulação de dados
- Matplotlib e Seaborn para visualizações
- Statsmodels para modelagem estatística
- Scikit-learn para divisão de dados e métricas de avaliação

Projeto no Colab: https://colab.research.google.com/drive/1EeB4Q0cDkEufrPIpxFW2o0ApYPKkMuPw?authuser=1
