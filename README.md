# MVP_Analise_de_Dados_e_Boas_Praticas

# Análise Exploratória e Pré-processamento de Dados Imobiliários

## Descrição do Projeto

Este projeto consiste em um MVP de Ciência de Dados com foco nas etapas iniciais de um pipeline analítico: Análise Exploratória de Dados (EDA) e Pré-processamento.

O objetivo é compreender a estrutura dos dados, identificar padrões, detectar problemas (como outliers e assimetrias) e preparar a base para futuras etapas de modelagem preditiva.

## Objetivo
- Explorar o comportamento das variáveis relacionadas ao preço de imóveis
- Identificar fatores potencialmente relevantes para previsão
- Tratar e preparar os dados para modelos de Machine Learning

## Base de Dados

O dataset contém 545 registros e 13 variáveis:

### Variável alvo:
- price — preço do imóvel
### Variáveis explicativas:
- area — área do imóvel
- bedrooms — número de quartos
- bathrooms — número de banheiros
- stories — número de andares
- parking — vagas de estacionamento
- mainroad — acesso à via principal
- guestroom — quarto de hóspedes
- basement — porão
- hotwaterheating — aquecimento de água
- airconditioning — ar-condicionado
- prefarea — área preferencial
- furnishingstatus — status da mobília

## Hipóteses Iniciais
- O preço do imóvel está fortemente relacionado à área
- Imóveis em áreas preferenciais tendem a ter preços mais elevados
- A presença de comodidades (garagem, ar-condicionado, etc.) impacta o valor

## Análise Exploratória (EDA)

Durante a análise, foram realizadas:

Estatísticas descritivas (média, mediana, desvio padrão)
Análise de distribuição das variáveis
Identificação de assimetria (principalmente em price e area)
Detecção de outliers
Avaliação de relações entre variáveis
Principais insights:
price e area apresentam distribuição assimétrica à direita
Variáveis possuem escalas muito diferentes
Existem valores extremos que podem impactar modelos futuros
Variáveis categóricas têm potencial explicativo relevante

## Pré-processamento dos Dados

Foram consideradas as seguintes etapas:

- Tratamento de variáveis categóricas (encoding)
- Avaliação da necessidade de:
Transformação logarítmica (price, area)
Padronização (StandardScaler)
Normalização (MinMaxScaler)
- Preparação dos dados para algoritmos de Machine Learning

## Próximos Passos

Construção de modelos preditivos
Teste de algoritmos como:
Regressão Linear
Random Forest
XGBoost
Avaliação de desempenho com métricas apropriadas

## Tecnologias Utilizadas

Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn

## Autor

Henrique Nunes
