# Multiple Linear Regression - Amsterdam Houses

Este projeto implementa um modelo de **Regressão Linear Múltipla** para prever o preço de imóveis em Amsterdã, utilizando variáveis como **área**, **número de quartos**, **latitude** e **longitude**.

## Estrutura do Projeto

* **Análise Exploratória de Dados (EDA)**: estatísticas descritivas, histogramas e boxplots para identificar tendências e outliers.
* **Preparação dos Dados**: seleção de variáveis, divisão em treino e teste.
* **Treinamento do Modelo**: uso do `LinearRegression` do `scikit-learn`.
* **Avaliação do Modelo**: cálculo do R² e interpretação dos coeficientes.
* **Interpretação dos Resultados**: análise de importância das variáveis e verificação de overfitting/underfitting.

## Tecnologias Utilizadas

Este notebook foi executado originalmente no Google Colab, mas também pode ser rodado localmente com:

* **Python 3**
* Bibliotecas:

  * `numpy`
  * `pandas`
  * `matplotlib`
  * `seaborn`
  * `scikit-learn`
  * `jupyter` (se for rodar localmente)

Para instalar todas as dependências de uma vez:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
```

## Dataset

O dataset usado foi **[Amsterdam Houses](https://www.kaggle.com/datasets/thomasnibb/amsterdam-house-price-prediction)**, contendo:

* `Area` — área total do imóvel (m²)
* `Rooms` — número de quartos
* `Longitude` — posição geográfica
* `Latitude` — posição geográfica
* `Price` — valor de venda do imóvel

## Resultados

* **Variável mais relevante**: Área
* **R² no teste**: \~0,774
  → O modelo explica cerca de **77% da variação** no preço dos imóveis.
* Não foi detectado overfitting ou underfitting significativos.

## Como Executar

1. Baixe o notebook `Multiple_Linear_Regression.ipynb`.
2. Certifique-se de ter o dataset `amsterdam_houses.csv` no caminho correto (ou ajuste o código para o local onde ele está).
3. Execute no Google Colab **ou** localmente:

   ```bash
   jupyter notebook Multiple_Linear_Regression.ipynb
   ```
4. Rode as células em ordem.
