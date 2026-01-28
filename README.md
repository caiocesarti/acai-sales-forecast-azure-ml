# 🍧 Previsão de Vendas de Açaí com Machine Learning no Azure
📌 Visão Geral

Este projeto tem como objetivo desenvolver um modelo de Machine Learning capaz de prever a demanda diária de açaí com base na temperatura, utilizando recursos do Azure Machine Learning.
A solução combina treinamento manual, pipelines visuais, Automated ML e infraestrutura em cloud, resultando em um projeto completo e reproduzível para portfólio profissional.

## 📊 Conteúdo

- **Análise Exploratória de Dados (EDA)**
- **Modelagem de Machine Learning**
- **Métricas e Avaliação de Modelos**
  

🧠 Contexto do Problema

Imagine uma loja de açaí localizada em uma cidade litorânea, onde as vendas variam significativamente conforme a temperatura.
Sem previsões confiáveis, o negócio pode sofrer com desperdício ou perda de vendas.
A aplicação de Machine Learning permite antecipar a demanda e apoiar decisões estratégicas de produção.

🎯 Objetivos do Projeto

- Prever vendas de açaí a partir da temperatura diária
- Treinar e avaliar um modelo de regressão
- Utilizar Azure Machine Learning como plataforma principal
- Explorar Notebook, Designer e Automated ML
- Documentar todas as etapas com evidências reais

☁️ Tecnologias Utilizadas

- Azure Machine Learning
- Python 3.10
- Pandas
- Scikit-learn
- MLflow
- Azure ML Designer
- Azure Automated ML

## 📋 Estrutura do Projeto

```
acai-ml/
├── acai-ml.ipynb          # Notebook principal com análise e modelos
├── src/
│   └── acai_sales.csv     # Dataset de vendas
├── evidence/              # Evidências e visualizações do projeto
└── README.md              # Este arquivo
```
🔧 Ambiente de Computação

O projeto foi executado em uma Compute Instance do Azure ML, garantindo ambiente isolado e adequado para experimentação.
Também foi configurado um Compute Cluster, utilizado para pipelines e execuções escaláveis.


📊 Registro do Dataset

O dataset foi registrado como Data Asset no Azure Machine Learning, permitindo versionamento e reutilização entre Notebook, Designer e AutoML.


📥 Carregamento do Dataset

O conjunto de dados foi carregado a partir de um arquivo CSV contendo data, temperatura e volume de vendas.


📈 Análise Exploratória

Foram analisadas estatísticas descritivas e estrutura dos dados, confirmando ausência de valores nulos e forte correlação entre temperatura e vendas.


🔀 Divisão Treino/Teste

Os dados foram divididos em 80% para treino e 20% para teste, garantindo avaliação adequada da generalização do modelo.


🤖 Treinamento do Modelo

Foi utilizado um modelo de Regressão Linear, treinado com sucesso no conjunto de treino.


📐 Avaliação do Modelo

O modelo apresentou excelente desempenho:

MAE: ~2 unidades

RMSE: ~2.6 unidades

R²: ~0.99

Esses resultados indicam alta precisão na previsão das vendas.


🧩 Pipeline no Azure ML Designer

O fluxo completo de Machine Learning também foi implementado no Azure ML Designer, utilizando componentes visuais para treino, pontuação e avaliação.

Execução do Pipeline

O pipeline foi executado com sucesso em cluster, com todas as etapas concluídas.


⚙️ Automated ML

Também foi executado um experimento com Azure Automated ML, que testou múltimos algoritmos automaticamente.
O melhor modelo identificado foi um Voting Ensemble, registrado via MLflow.


🏁 Conclusão

O projeto demonstra, de forma prática, a aplicação de Machine Learning em um cenário real de negócio, utilizando recursos completos do Azure Machine Learning.


🚀 Possíveis Evoluções

Inclusão de variáveis climáticas adicionais

Uso de modelos de séries temporais

Deploy do modelo como endpoint de inferência

Monitoramento de desempenho em produção



## 🚀 Como Usar

1. Clone o repositório:
```bash
git clone https://github.com/[seu-usuario]/acai-ml.git
```

2. Acesse o diretório:
```bash
cd acai-ml
```

3. Abra o notebook:
```bash
jupyter notebook acai-ml.ipynb
```

## 📁 Arquivos

- `acai-ml.ipynb` - Análise principal e treinamento de modelos
- `src/acai_sales.csv` - Dataset com informações de vendas
- `evidence/` - Imagens e evidências dos resultados

## 🛠️ Requisitos

- Python 3.x
- Jupyter Notebook
- pandas
- scikit-learn
- matplotlib
- seaborn

## 📜 Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo [LICENSE](LICENSE) para mais informações.

## ✨ Autor

Desenvolvido por Caio Cesar
caiocesadeveloper@gmail.com
