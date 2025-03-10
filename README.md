# 🏠 Prevendo Valores de Imóveis com Regressão Linear

Este projeto tem como objetivo precificar o valor de venda de imóveis utilizando um modelo de Regressão Linear. Além disso, exploramos quais fatores melhor explicam o valor dessas propriedades, permitindo uma melhor compreensão do mercado imobiliário.

## 📌 Etapas do Projeto

O projeto foi desenvolvido seguindo os seguintes passos:

1. 📥 **Importação das Bibliotecas**: Utilização de bibliotecas essenciais para análise de dados e machine learning.
2. 📂 **Carregamento dos Dados**: Importação e inspeção do conjunto de dados.
3. 🔄 **Pré-processamento**:
   - ❌ Remoção de colunas irrelevantes (exemplo: ID dos imóveis).
   - 🛠️ Tratamento de valores nulos e inconsistentes.
4. 📊 **Análise Exploratória**:
   - 🔎 Cálculo da correlação entre as variáveis.
   - 📉 Visualização de distribuições e relações entre variáveis.
5. ✂️ **Divisão dos Dados**:
   - 📏 Separar os dados em conjunto de treino e teste.
6. 🤖 **Treinamento do Modelo**:
   - 🔢 Aplicar a Regressão Linear para prever os preços de venda.
7. 📈 **Avaliação do Modelo**:
   - 📌 Cálculo de métricas de desempenho para avaliar a qualidade do modelo.

## 💾 Como Baixar e Executar o Projeto

### 🔧 Requisitos

- 🐍 Python 3.7+
- 📦 Bibliotecas listadas no arquivo `requirements.txt`
- 🏗️ (Opcional) Anaconda para gerenciamento de ambientes

### 🚀 Instalação

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/prevendo-valores-imoveis.git
   ```
2. Acesse a pasta do projeto:
   ```bash
   cd prevendo-valores-imoveis
   ```
3. Crie um ambiente virtual e instale as dependências:
   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows, use venv\Scripts\activate
   pip install -r requirements.txt
   ```
4. Execute o Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
5. Abra o arquivo `.ipynb` e execute as células.

## ✨ Possíveis Melhorias

- 🏗️ Testar outros modelos de regressão (Ex: Regressão Ridge, Lasso, Random Forest Regressor).
- 🔍 Explorar feature engineering para melhorar a previsão.
- 🤖 Implementar um pipeline automatizado para treinamentos futuros.
- 🌐 Criar uma API para disponibilizar as previsões de forma online.

## 🤝 Contribuição

Caso queira contribuir com melhorias, fique à vontade para abrir um PR ou sugerir mudanças via issues.

## 📜 Licença

Este projeto está sob a licença MIT. Sinta-se livre para usá-lo e melhorá-lo!

