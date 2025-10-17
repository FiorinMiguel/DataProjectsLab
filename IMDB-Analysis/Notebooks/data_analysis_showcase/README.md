# Exploração de Dados com SQL - IMDB

## Descrição

Análise exploratória do banco de dados IMDB (Internet Movie Database) desenvolvida para o laboratório da disciplina ME315. O projeto investiga padrões em filmes, avaliações e participantes através de consultas SQL e análise de dados em Python.

## Objetivos

- Explorar a estrutura do banco de dados IMDB
- Identificar os filmes melhor avaliados
- Analisar distribuição de gêneros em filmes de alta avaliação
- Descobrir atores/atrizes mais frequentes em filmes bem avaliados

## Estrutura do Banco de Dados

**Tabelas principais:**
- `basics`: Informações básicas dos títulos
- `ratings`: Avaliações dos usuários
- `principals`: Relação entre títulos e participantes

## Análises Realizadas

1. **Top 5 Filmes Melhor Avaliados**
   - Critério inicial: maior averageRating
   - Critério refinado: averageRating + numVotes > 100.000

2. **Gênero Mais Frequente em Filmes com Nota > 8**
   - Análise de distribuição de gêneros
   - Investigação de fatores que influenciam avaliações

3. **Atores/Atrizes em Filmes com Nota > 7.5**
   - Contagem de participações em filmes bem avaliados

## Tecnologias Utilizadas

- Python 3
- SQLite
- pandas
- Jupyter Notebook
- SQL

## Arquivos

- `analise_imdb.ipynb` - Jupyter Notebook com análise completa
- `analise_imdb.html` - Versão HTML do notebook
- `IMDB.db` - Banco de dados (não incluído)
- `README.md` - Documentação

## Como Executar

1. Instalar dependências:
```bash
pip install pandas sqlite3 jupyter
