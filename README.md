# README – Notebook Colab

## 1. Visão Geral

Este notebook automatiza a integração de dados entre um arquivo CSV (lista de preços enviada pela HP) e um banco de dados SQLite (dados extraídos do Mercado Livre via Selenium). Ao final, gera relatórios técnicos em PDF e Word contendo análises descritivas, visuais e documentação do processo.

## 2. Requisitos

- Python 3.x (já disponível no Colab)
- Biblioteca pandas
- Biblioteca matplotlib
- Biblioteca reportlab
- Biblioteca python-docx
- Módulo sqlite3 (incluso no Python)

## 3. Estrutura do Notebook

1. **Instalação de Dependências**\
   Instalação de pacotes necessários via `pip`.
2. **Importação de Bibliotecas**\
   Carrega pandas, matplotlib, reportlab, python-docx e sqlite3.
3. **Carregamento dos Dados**
   - Upload de `Lista de preços.csv`
   - Upload de `mercadolivre.db`
   - Leitura em DataFrame e em banco SQLite.
4. **Integração dos Dados**
   - Identificação de colunas em comum
   - Merge ou concatenação lateral
   - Descrição da estratégia adotada.
5. **Tratamento e Criação de Colunas Derivadas**
   - Normalização de valores de preço
   - Conversão para float
   - Geração de estatísticas descritivas.
6. **Análise Descritiva e Visual**
   - Estatísticas de `preco_numerico`
   - Histograma da distribuição de preços.
7. **Geração de Relatórios**
   - Geração de PDF (`relatorio_tecnico.pdf`)
   - Geração de Word (`relatorio_tecnico.docx`)
   - Salvamento dos arquivos no ambiente do Colab.
8. **Conclusão**\
   Sumário dos resultados e próximos passos para enriquecimento de dados.

## 4. Como Executar

1. Abra este notebook no Google Colab.
2. Faça upload dos arquivos:
   - `Lista de preços.csv`
   - `mercadolivre.db`
3. Execute cada célula em ordem (use `Ctrl+F9` para executar todas).
