🎯 Objetivo do Projeto
O problema de negócio central é migrar a área de Prevenção de Perdas de uma abordagem reativa (analisando perdas que já ocorreram) para uma estratégia proativa e preditiva. O pipeline construído permite:

Centralizar os dados de perdas, transporte e segurança em um Data Warehouse na nuvem (BigQuery).

Analisar as principais causas de perdas por diversas dimensões (Motivo, Local, Categoria, Rota).

Detectar anomalias e correlações suspeitas entre eventos de segurança e perdas.

Gerar resumos estratégicos automáticos usando uma simulação de IA generativa (Gemini).

Visualizar todos os KPIs e insights em um dashboard executivo e automatizado no Looker Studio, com envio programado de relatórios por e-mail.

🛠️ Tecnologias e Sistemas Utilizados
Linguagem: Python 3

Bibliotecas Principais:

pandas: Para manipulação de dados.

duckdb: Para análises SQL exploratórias em arquivos CSV locais.

google-cloud-bigquery: Para interagir (ler e escrever) com o BigQuery.

google-auth: Para autenticação segura com o Google Cloud.

Data Warehouse: Google BigQuery

Visualização (BI): Looker Studio (antigo Google Data Studio)

Autenticação: Google Cloud CLI (gcloud)

Inteligência Artificial: Simulação da API do Google Gemini para geração de texto.

📂 Estrutura do Repositório
/Prevencao_de_Perdas
|
|--- 📂 data_generation/
|    |--- generate_product_catalog.py
|    |--- generate_loss_events.py
|    |--- ... (outros scripts de geração)
|
|--- 📂 data/
|    |--- product_catalog.csv
|    |--- loss_events.csv
|    |--- ... (arquivos CSV gerados)
|
|--- 📂 01_Desafio_Analise_Causa_Raiz/
|    |--- 01_analise_exploratoria.py
|
|--- 📂 02_Desafio_Deteccao_de_Anomalias/
|    |--- 02_investigacao_de_padroes.py
|
|--- 📂 05_Desafio_Insights_com_IA_Generativa/
|    |--- 05_gerador_de_insights_real.py
