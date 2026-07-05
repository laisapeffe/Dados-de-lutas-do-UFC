# Dados-de-lutas-do-UFC
Este MVP faz parte do sprint de  Machine Learning e Analitycs do curso de Pós-Graduação em Ciência de Dados e Analytics da PUC-Rio.

## Objetivo

Testar se modelos não-lineares/ensemble (Random Forest e XGBoost) superam um baseline simples ao capturar interações entre variáveis pré-luta, prevendo o resultado (`red_winner`) sem uso de dados que só existem após o evento.

## Estrutura esperada do projeto

```
.
├── mvp_ml_analytics.ipynb     # notebook principal (análise, pré-processamento, treino e avaliação)
├── all_fights.csv          # dataset de entrada (não incluso no repositório)
└── README.md
```

## Pré-requisitos

- Python 3.9 ou superior
- pip

## Instalação

1. Clone ou baixe este repositório.
2. (Recomendado) Crie um ambiente virtual:
   ```bash
   python3 -m venv venv
   source venv/bin/activate      # Linux/Mac
   venv\Scripts\activate         # Windows
   ```
3. Instale as dependências:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly scikit-learn xgboost
   ```

## Obtendo o dataset

O projeto utiliza o dataset **UFC Fight Data 2026**, disponível publicamente no Kaggle:
🔗 https://www.kaggle.com/datasets/anthonysz/ufc-fight-data-2026/data

Baixe o arquivo `all_fights.csv` e coloque-o na raiz do projeto (ou ajuste o caminho no script, conforme o passo abaixo).

## Configuração do caminho do dataset

O script foi originalmente escrito para rodar no Google Colab, lendo o dataset diretamente do GitHub:
