
🛠️ Etapas Realizadas
⚙️ 1. Ambiente e Sessão PySpark
Instalação do PySpark via pip.

Configuração de variáveis de ambiente para compatibilidade com o Python.

Criação da SparkSession com o nome PySpark_01.

📂 2. Leitura do Dataset
Leitura do arquivo .csv com spark.read.csv(), utilizando:

header=True para reconhecer cabeçalhos.

inferSchema=True para inferência automática dos tipos.

Exibição inicial dos dados com df.show() e estrutura com df.printSchema().

🧪 3. Análise de Dados Nulos
Conversão para DataFrame Pandas: df.toPandas().isna().sum() para detectar colunas com valores ausentes.

Verificação com PySpark usando filter() e count() para checar linhas nulas diretamente no ambiente distribuído.

🧹 4. Tratamento de Dados
Renomeação de colunas com caracteres especiais, facilitando manipulação (ex: Pos. → Posicao, # → Numero, Club → Time).

Padronização para nomes descritivos em snake_case.

