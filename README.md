# b3-energy-stocks-ml-prediction

[](https://www.python.org/)
[](https://pandas.pydata.org/)
[](https://scikit-learn.org/stable/)
[](https://pypi.org/project/yfinance/)
[](https://www.databricks.com/pt-br/try-databricks)
[](https://opensource.org/licenses/MIT)

## 📊 Descrição do Projeto

Este projeto tem como objetivo desenvolver um modelo de Machine Learning (ML) para prever a tendência de preço de ações específicas do Setor de Energia listadas na B3 (Bolsa de Valores do Brasil). Serve como uma peça de portfólio para demonstrar habilidades em coleta, engenharia, análise e modelagem de dados financeiros.

## 🎯 Objetivo Principal

Criar um protótipo de um sistema de previsão para determinar se o preço de fechamento de uma ação do setor de energia na B3 irá subir (tendência de alta) ou descer (tendência de baixa) no dia seguinte.

## ✨ Etapas da Prototipagem (Metodologia)

Este projeto segue uma abordagem estruturada, dividida nas seguintes fases iniciais:

### 1. Seleção dos Ativos (Nicho)
-   **Ação:** Escolha de 3 a 5 tickers de empresas de energia negociadas na B3.
-   **Exemplos:** ENBR3, EGIE3, TRPL4, CMIG4, CPFE3.

### 2. Coleta de Dados
-   **Ação:** Utilização da biblioteca `yfinance` do Python para baixar a série histórica de preços (fechamento, abertura, máxima, mínima, volume) dos ativos selecionados.
-   **Período:** Definição de um período histórico relevante (ex: 5 a 10 anos de dados diários).
-   **Armazenamento:** Os dados brutos serão salvos em um formato comum (CSV ou Parquet) para reusabilidade.

### 3. Análise Exploratória de Dados (EDA)
-   **Ação:** Notebooks dedicados para:
-   Cálculo e visualização de Retornos Diários e Volatilidade.
-   Verificação de dados ausentes, tratamento de outliers e análise de consistência.
-   Criação de gráficos de linha da série histórica de preços para identificar padrões.
-   **Ambiente:** Databricks Community Edition (para escalabilidade e notebooks interativos) ou ambiente local (Jupyter Notebooks).

### 4. Engenharia de Variáveis (Features)
-   **Ação:** Cálculo de indicadores técnicos que servirão como variáveis de entrada para o modelo de ML.
-   **Exemplos de Indicadores:**
-   Médias Móveis Simples (MMS) e Exponenciais (MME).
-   Índice de Força Relativa (RSI).
-   Média Móvel Convergência Divergência (MACD).
-   Volatilidade (ex: desvio padrão de retornos).

### 5. Definição do Problema (Target)
-   **Ação:** Clarificação do que o modelo tentará prever.
-   **Target (Classificação):** A ação sobe (1) ou desce (0) no dia seguinte (com base no preço de fechamento).
-   **Target (Regressão - Opcional para futura expansão):** O preço exato de fechamento no dia seguinte.

### 6. Protótipo ML Básico
-   **Ação:** Treinamento e teste de um algoritmo de Machine Learning para prever o target definido.
-   **Algoritmos Considerados:** Regressão Logística, Random Forest, ou outros modelos de classificação.
-   **Métricas:** Avaliação da performance do modelo usando métricas apropriadas (ex: Acurácia, Precisão, Recall, F1-Score, ROC AUC).
-   **Ambiente:** Databricks Community Edition ou ambiente local.

## 🛠️ Tecnologias Utilizadas

-   **Linguagem:** Python (3.9+)
-   **Coleta de Dados:** `yfinance`
-   **Manipulação de Dados:** `pandas`, `numpy`
-   **Análise e Visualização:** `matplotlib`, `seaborn`
-   **Machine Learning:** `scikit-learn`
-   **Ambiente de Desenvolvimento:** Databricks Community Edition / Jupyter Notebooks
-   **Controle de Versão:** Git / GitHub

## 📂 Estrutura do Projeto
