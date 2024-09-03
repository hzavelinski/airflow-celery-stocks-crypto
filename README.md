# Projeto de Pipelines de Dados com Airflow e Celery

Este projeto demonstra a construção de pipelines de dados utilizando Apache Airflow e Celery para orquestração e agendamento de tarefas. O objetivo é coletar, processar e salvar cotações diárias de ações e criptomoedas em formato CSV localmente.

## 📝 Visão Geral do Projeto

### Objetivos
1. **Coletar Dados:** Extrair cotações diárias de ações e criptomoedas de APIs públicas e salvar localmente em formato CSV.
2. **Processar e Armazenar:** Transformar os dados e salvá-los localmente em formato CSV.

## 🛠️ Tecnologias Utilizadas
* **Apache Airflow:** Para orquestração e agendamento de tarefas.
* **Celery:** Para gerenciamento de tarefas assíncronas no Airflow.

## 🏗️ Arquitetura do Pipeline
* **Extração:** Uma tarefa no Airflow coleta cotações diárias de ações e criptomoedas das APIs públicas.
* **Transformação:** Os dados brutos extraídos são processados e transformados em formato CSV.
* **Armazenamento:** Os dados transformados são armazenados localmente nas pastas `data/stocks` e `data/crypto`.


## 📥 Instalação e Configuração

1. **Configurar o Apache Airflow com Celery:**
   - Instale o Apache Airflow e Celery.
   - Configure o `airflow.cfg` para usar o Celery como executor.

2. **Instalar Dependências:**
   - Instale as dependências necessárias para o Airflow.

3. **Executar o Pipeline:**
   - Inicie o servidor do Airflow e o worker do Celery.
   - Execute os DAGs para iniciar o processo de coleta e transformação de dados.


## 🔗 Referências

* [Documentação do Apache Airflow](https://airflow.apache.org/)
* [Documentação do Celery](https://docs.celeryproject.org/)


