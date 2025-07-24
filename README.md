
🛠️ ##Etapas Realizadas##

1 - Ambiente e Sessão PySpark

Instalação do PySpark (pip install pyspark).

Configuração das variáveis de ambiente para evitar conflitos de versão com o Python.

Criação da SparkSession com o nome PySpark_01.

2 - Leitura do Dataset

Utilizado arquivo CSV com dados dos jogadores da Copa.

Leitura com spark.read.csv() utilizando header=True e inferSchema=True para detectar automaticamente os tipos de dados.

Exibição inicial do conteúdo com df.show() e esquema com df.printSchema().

3 - Análise de Dados Nulos

Conversão para Pandas para contagem de valores nulos: df.toPandas().isna().sum().

Iteração com filter().count() para identificar colunas com valores nulos diretamente no PySpark.

4 - Tratamento de Dados

Renomeação de colunas para remover caracteres especiais e facilitar o manuseio (ex: Pos. → Posicao, # → Numero, Club → Time).

Criação de novas colunas com nomes mais intuitivos e no padrão snake_case.
