# Análise Estratégica de Conteúdo da Netflix

Este projeto realiza uma análise estratégica do catálogo de conteúdos da Netflix, utilizando dados públicos para entender a evolução do portfólio, distribuição de tipos de conteúdo, gêneros e países produtores.

O foco do projeto é estruturar um pipeline analítico completo, com ênfase em SQL analítico e visualização de dados para apoiar decisões estratégicas relacionadas a conteúdo.

A arquitetura do projeto segue o padrão **Medallion (Bronze, Silver e Gold)**, separando claramente dados brutos, tratados e analíticos.

Fonte dos dados:
https://www.kaggle.com/datasets/shivamb/netflix-shows

---

## Objetivo do Projeto

- Analisar a composição e evolução do catálogo da Netflix
- Identificar padrões por tipo de conteúdo (Filmes vs Séries)
- Avaliar a distribuição de gêneros e países produtores
- Construir KPIs estratégicos para apoio à decisão
- Desenvolver dashboards analíticos no Power BI
- Demonstrar domínio de SQL analítico em um projeto real

---

## Perguntas de Negócio Respondidas

- Qual a proporção entre Filmes e Séries no catálogo?
- Como o catálogo evoluiu ao longo do tempo?
- Quais gêneros dominam o portfólio?
- Quais países mais produzem conteúdo para a Netflix?
- Onde há concentração ou diversificação de conteúdo?

---

## Ferramentas Utilizadas

- Python (Pandas)
- Jupyter Notebook (Google Colab)
- SQL (PostgreSQL)
- Power BI
- Git e GitHub

---

## Arquitetura de Dados (Medallion)

- **Bronze**: dados brutos do Kaggle, sem transformações
- **Silver**: dados tratados, normalizados e preparados para análise
- **Gold**: dados analíticos, KPIs e visões prontas para BI

Cada camada possui documentação específica no repositório.

---

## Estrutura do Repositório

```text
netflix-content-analytics/
│
├── 01_bronze/
│ ├── README.md
│ └── raw/
│ └── netflix_titles.csv
│
├── 02_silver/
│ ├── README.md
│ ├── notebooks/
│ │ └── 01_eda_tratamento_conteudo.ipynb
│ └── processed/
│ ├── netflix_titles_silver.csv
│ ├── netflix_genres.csv
│ └── netflix_countries.csv
│
├── 03_gold/
│ ├── README.md
│ ├── sql/
│ │ ├── 01_views_base.sql
│ │ ├── 02_kpis_catalogo.sql
│ │ ├── 03_kpis_temporais.sql
│ │ └── 04_kpis_regionais.sql
│ └── power_bi/
│ └── netflix_dashboard.pbix
│
└── images/
```
---

## Resultados Esperados

- Análise de mais de **8.000 títulos**
- KPIs estratégicos sobre portfólio de conteúdo
- Dashboards voltados à tomada de decisão
- Projeto documentado e reproduzível

---

## Como Reproduzir o Projeto

1. Baixar o dataset no Kaggle
2. Executar o notebook de tratamento (Silver)
3. Carregar os dados tratados no PostgreSQL
4. Executar os scripts SQL (Gold)
5. Abrir o dashboard no Power BI
