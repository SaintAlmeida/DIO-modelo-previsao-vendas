# Modelo de Previsão de Vendas com Azure Machine Learning

Este projeto demonstra a criação de um modelo de machine learning simples para previsão de vendas e a configuração dos seus respectivos pontos de extremidade (endpoints) para consumo via API.

## 🧠 Etapa 1: Criação do modelo

1. Acesse o portal [Azure Machine Learning Studio](https://ml.azure.com).
2. Crie um novo **workspace**.
3. Vá para "Designer" e selecione um pipeline em branco.
4. Importe o conjunto de dados (por exemplo: histórico de vendas em CSV).
5. Aplique os seguintes passos no pipeline:
   - **Select Columns in Dataset**
   - **Split Data** (80% treino / 20% teste)
   - **Train Model** (algoritmo: Linear Regression)
   - **Score Model**
   - **Evaluate Model**
6. Execute o pipeline.

## ⚙️ Etapa 2: Criação do endpoint

1. Após o treinamento, publique o pipeline como um **serviço**.
2. Vá para “Endpoints” > “Real-time endpoints”.
3. Anote as seguintes informações:
   - URL do endpoint
   - Chave de autenticação
   - Parâmetros de entrada e saída

Esses dados estão descritos no arquivo `endpoint-config.json`.

## 🧾 Etapa 3: Estrutura do repositório

