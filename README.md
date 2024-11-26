# Rotatividade de Clientes

## 📋 Descrição do Projeto

A operadora de comunicações InternetGO está interessada em prever a rotatividade de seus clientes (churn). Se for identificado que um usuário está planejando trocar de operadora, a empresa poderá oferecer códigos promocionais e opções de planos especiais para evitar a perda desse cliente. Será desenvolvido um modelo capaz de identificar precocemente clientes com maior probabilidade de cancelamento, permitindo ações preventivas de retenção

A equipe de marketing da InternetGO coletou dados pessoais de seus clientes, incluindo informações sobre seus planos e contratos.

## 📊 Serviços da InternetGO

A InternetGO oferece principalmente dois tipos de serviços:

1. Telefonia fixa: O telefone pode ser conectado a várias linhas simultaneamente.
2. Internet: A rede pode ser estabelecida via linha telefônica (DSL) ou cabo de fibra óptica.

Além disso, a empresa também fornece serviços adicionais, como:

- Segurança na Internet: antivírus (DeviceProtection) e bloqueador de sites maliciosos (OnlineSecurity)
- Suporte técnico dedicado (TechSupport)
- Armazenamento de arquivos na nuvem e backup de dados (OnlineBackup)
- Streaming de TV (StreamingTV) e diretório de filmes (StreamingMovies)

Os clientes podem escolher entre pagamento mensal ou contratos de 1 ou 2 anos, com diversos métodos de pagamento e fatura eletrônica.

Descrição dos Dados

## 🛠️ Ferramentas e Bibliotecas Utilizadas
- Python: Linguagem principal utilizada para a análise.
- Pandas e Numpy: Biblioteca para manipulação e análise de dados.
- Sklearn e Catboost Biblioteca para construção de modelo de machine learning.
- Matplotlib.pyplot e Seaborn: Biblioteca para construção de gráficos

## 📊 Os dados fornecidos para este projeto final incluem:

- `contract.csv`: Informações contratuais
- `personal.csv`: Dados pessoais dos clientes
- `internet.csv`: Informações sobre serviços de Internet
- `phone.csv`: Informações sobre serviços telefônicos

Todas as informações estão relacionadas a partir de 1º de fevereiro de 2020, com o `customerID` como identificador único de cada cliente.

## 🔍 Aprendizados

- `Análise de dados`: interpretação e extração de insights valiosos a partir de grandes volumes de dados.
- `Preparação do conjunto para aplicações em Machine Learning`: separação do conjunto original em teste e treino, além da seleção das features e target do modelo.
- `Funções`: construção e aplicação de funções para simplificar o código.
-  `Regras de negócios`: aplicação de regras de negócio para resolução de problemas.
-  `Aplicação de modelos de Machine Learning`: aplicação, seleção de hiperparâmetros, teste e avalição do modelo.
-  `Documentação de projetos`: elaboração de documentação clara e detalhada para garantir que o projeto seja compreensível e replicável.
- `Utilização de bibliotecas e ferramentas`: aplicação prática de diversas bibliotecas e ferramentas do ecossistema Python.
- `Tomada de decisões baseadas em dados`: uso de insights derivados da análise de dados para orientar decisões estratégicas.

## 📈 Conclusão

Realizamos todo o processo passo a passo para treinar o modelo. Todos os inconvenientes encontrados foram facilmente resolvidos durante a Análise Exploratória de Dados (EDA), como a conversão de colunas, criação da coluna alvo "churn" como variável binária, e a realização de encoding e escalonamento antes de treinar os modelos testados. O projeto foi dividido em duas etapas principais: a primeira foi a EDA, onde conseguimos entender os dados e analisar as possíveis causas do problema; a segunda foi o ajuste de hiperparâmetros, onde garantimos que o modelo alcançasse uma alta pontuação AUC tanto no conjunto de teste quanto no conjunto de validação, para resolver o problema que identificamos.

o modelo com melhor desempenho foi: catboost com AUC-ROC: 0.9160921181462143


## 🚀 Como Usar

1. Clone o repositório
```bash
 https://github.com/paulo-santos-ds/rotatividade_de_clientes
```

2. Extrair o arquivo (imdb_reviews.zip)

3. Instale as dependências
```bash
pip install -r requirements.txt
```

4. Execute o notebook principal
```bash
rotatividade_de_clientes.ipynb
```
