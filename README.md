# Python Insights — Cancelamento de Clientes 📉

Um projeto de **análise de dados** que simula um cenário extremamente comum em empresas: **entender por que clientes estão cancelando** e **o que pode ser feito para reduzir o cancelamento (churn)** usando dados reais (ou realistas) e **decisões orientadas por evidências**.

---

## 🎯 Objetivo do Projeto

O **Python Insights — Cancelamento de Clientes** tem como objetivo transformar dados brutos em decisões claras, respondendo perguntas como:

- **Quem** está cancelando?
- **Quando** o cancelamento acontece com mais frequência?
- **Quais características** (perfil, uso, contrato, pagamento, atendimento etc.) aumentam a chance de churn?
- **Quais ações** teriam maior impacto para reduzir cancelamentos?

Este projeto é ideal para portfólio, estudos de análise exploratória (EDA) e construção de raciocínio analítico voltado para o negócio.

---

## 🧠 Contexto (problema de negócio)

Em muitas empresas, aumentar vendas é caro — já **reduzir churn** costuma ser uma das formas mais eficientes de crescer.

A lógica é simples:
- **Churn alto** → receita instável, CAC “se perde”, previsão de crescimento vira loteria.
- **Churn baixo** → base cresce com mais consistência, mais upsell/cross-sell, mais previsibilidade.

Aqui, a meta não é “fazer gráficos bonitos”: é **gerar insights acionáveis** para priorizar melhorias e orientar decisões.

---

## 🔎 O que você vai encontrar aqui

### 1) Preparação e qualidade de dados
- Leitura de dados (incluindo suporte a Excel com `openpyxl`)
- Tipagem e padronização de colunas
- Tratamento de valores ausentes e inconsistentes
- Checagens rápidas de qualidade (ex.: duplicidades, ranges improváveis)

### 2) Análise Exploratória (EDA)
- Visão geral da base: distribuição do alvo (cancelou vs. não cancelou)
- Perfil dos clientes com maior churn
- Comparações por variáveis relevantes (categorias e numéricas)
- Exploração de correlações e padrões

### 3) Visualizações para decisão (Plotly)
- Gráficos interativos focados em:
  - Taxa de churn por segmento
  - Impacto de contrato, método de pagamento, tempo de casa, uso/consumo
  - Identificação de “zonas de risco” (ex.: clientes recém-entrados)

### 4) Conclusões e recomendações
- Resumo dos principais fatores associados ao cancelamento
- Sugestões de ações práticas (ex.: melhorias de onboarding, ofertas de retenção, revisão de planos)
- Priorização do que tende a trazer mais impacto

> A ideia é sair do “parece que…” e chegar no “os dados sugerem que…”.

---

## 🧰 Tecnologias e bibliotecas

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![ipykernel](https://img.shields.io/badge/ipykernel-000000?style=for-the-badge&logo=jupyter&logoColor=white)
![nbformat](https://img.shields.io/badge/nbformat-4B8BBE?style=for-the-badge&logo=python&logoColor=white)
![openpyxl](https://img.shields.io/badge/openpyxl-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

---

# Clonar o repositório
``git clone https://github.com/seuusuario/python-insights-cancelamento-clientes.git``
<br>
``cd python-insights-cancelamento-clientes``

# Criar e ativar um ambiente virtual

# Windows

``python -m venv .venv``
<br>
``.venv\Scripts\activate``

# MacOS/Linux
``python3 -m venv .venv``
<br>
``source .venv/bin/activate``

# Instalar dependências
Se você tiver um ``requirements.txt``:
``pip install -r requirements.txt``

Ou instale manualmente:
``pip install pandas numpy plotly openpyxl ipykernel nbformat jupyter``

# Rodar o Jupyter
``jupyter notebook``

# 📌 Principais perguntas respondidas (exemplos)

- Clientes com pouco tempo de casa cancelam mais?
- Algum tipo de contrato (mensal/anual) tem churn significativamente maior?
- Existe relação entre preço/valor mensal e cancelamento?
- Método de pagamento ou atrasos são sinais de risco?
- Há segmentos que merecem estratégias diferentes (retenção por cluster/segmento)?

# ✅ Entregáveis

- Notebook com a análise completa e reproduzível
- Visualizações interativas para explorar segmentos
- Lista de insights e recomendações acionáveis
- (Opcional) Export de gráficos e um mini-relatório em outputs/reports/

# 🧩 Como adaptar para sua realidade

Se você quiser deixar esse projeto mais “cara de empresa”, algumas evoluções naturais são:

- Criar uma métrica de risco de churn (score simples por regras)
- Adicionar análise de coorte (churn por mês de entrada)
- Criar um dashboard (Plotly/Dash ou Streamlit)
- Implementar um pipeline mais organizado (funções no ``src/``)

# 🤝 Contribuição

Sugestões e melhorias são bem-vindas!

- Abra uma issue com ideias/bugs
- Envie um pull request com melhorias no notebook, visualizações ou organização do projeto
