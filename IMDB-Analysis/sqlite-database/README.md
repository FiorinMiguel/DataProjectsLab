# IMDb Data Processing

> Processamento de 88M+ registros com R + SQLite + Chunking

## Resultados
- **88.359.623** registros processados  
- **3.8 GB** de dados transformados  
- **0 travamentos** com 8 GB RAM  
- Banco **SQLite** otimizado  

## Tech
`R` `SQLite` `RSQLite` `readr` `Chunking`

## Download
[![Google Drive](https://img.shields.io/badge/🗃️_IMDB.db_(4.5GB)-4285F4?style=for-the-badge)](https://drive.google.com/drive/folders/1ccBQFQNY67_s6kYwD3JioiZ3VHNv7K-N?usp=drive_link)

## Arquivos
- `criacao_banco_sqlite.qmd` — Pipeline completo de ETL  

---

## Pré-processamento de dados

Durante a importação dos arquivos originais da IMDb, foi identificado que o arquivo `title.ratings.tsv` apresentava **inconsistências de separadores** (mistura de tabulações e espaços).  
Para padronizar o formato e garantir a leitura correta no R, foi aplicado o seguinte comando no Ubuntu:

```bash
awk '{$1=$1}1' OFS='\t' title.ratings.tsv > title.ratings_fixed.tsv
