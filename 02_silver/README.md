\# Camada Silver — Dados Tratados



A camada Silver é responsável pela limpeza, padronização e normalização dos dados brutos, preparando-os para análises analíticas.



Nesta etapa, os dados deixam de ser apenas registros e passam a ser estruturados de forma analítica.



\## Atividades Realizadas



\- Limpeza de campos textuais

\- Conversão de tipos de dados

\- Padronização de datas

\- Normalização de colunas com múltiplos valores (gêneros e países)

\- Criação de tabelas auxiliares (dimensões)



\## Conteúdo da Pasta



\- `notebooks/`

&nbsp; - Notebook de EDA e tratamento (`01\_eda\_tratamento\_conteudo.ipynb`)

\- `processed/`

&nbsp; - `netflix\_titles\_silver.csv`

&nbsp; - `netflix\_genres.csv`

&nbsp; - `netflix\_countries.csv`



\## Versionamento



\- Notebooks e dados tratados são versionados para facilitar reprodutibilidade

\- Dados tratados refletem regras de negócio e decisões analíticas



\## Responsabilidade da Camada



\- Garantir consistência e qualidade dos dados

\- Definir granularidade correta para análises

\- Preparar dados para consumo em SQL



