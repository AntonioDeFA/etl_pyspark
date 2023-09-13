## README.md

---

# Transformação de Dados: IBGE e Casos de COVID

Este repositório aborda a transformação de dados das cidades brasileiras (IBGE) e casos de COVID. Foram criados dois projetos independentes para realizar transformações nos dados, um usando PySpark e o outro usando Pyspark focando em integração com SQL. O objetivo é limpar, preparar e combinar os dados para análises subsequentes.

## Projetos

### 1. **PySpark**

Localizado no arquivo `Dados_IBGE_pyspark.ipynb`. Esse projeto foi construído usando a biblioteca PySpark e realiza as seguintes operações:

- Carregamento dos dados.
- Remoção de acentos nas cidades.
- Separação do nome da cidade e estado.
- Junção das massas de dados do IBGE e casos de COVID.
- Renomeação das colunas para português.
- Exportação dos dados transformados para um CSV.

### 2. **Scala**

Localizado no arquivo `Dados_IBGE.ipynb`. Ele segue a mesma ideia do anterior, porém focado com integração com SQL

## Fontes de Dados

1. **Dados do IBGE**: Contém informações demográficas sobre diferentes cidades do Brasil.
2. **Casos de COVID**: Informações sobre casos confirmados, mortes e outras métricas relacionadas à COVID-19 em diferentes cidades do Brasil.

## Como Executar

1. **Preparação**:
   
   Instale as bibliotecas necessárias:
   ```bash
   pip install pyspark findspark unidecode
   ```

2. **Execução**:

   - Para o projeto PySpark: Execute o script `Dados_IBGE_pyspark.ipynb` ou `Dados_IBGE.ipynb`.

## Resultados

Os resultados transformados são armazenados em um arquivo CSV chamado `relatorio-final.csv`, que pode ser usado para análises posteriores.
