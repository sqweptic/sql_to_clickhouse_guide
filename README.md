# Checking csv dataset

- [Checking csv dataset](#checking-csv-dataset)
  - [Guide to converting SQL queries to clickhouse systax queries (which pseudo-sql)](#guide-to-converting-sql-queries-to-clickhouse-systax-queries-which-pseudo-sql)
      - [Used datasets source](#used-datasets-source)
      - [Try by yourself](#try-by-yourself)

## Guide to converting SQL queries to clickhouse systax queries (which pseudo-sql)

Clickhouse queries syntax is quite unusual compared to common sql (sql-92 / sql-03 and so on).
So here is the guide to help switching your common sql queries to clickhouse syntax.


#### Used datasets source
* Bank accounts dataset - [Kaggle](https://www.kaggle.com/apoorvwatsky/bank-transaction-data)

#### Try by yourself
Easiest way to execute queries from the guide from scratch is follow: 
1. Run common sql syntax db docker container. 
Presto for example as it's quite powerful for the analytical purposes and it can be used with many databases through connectors. 
https://hub.docker.com/r/prestosql/presto
2. Run clickhouse-server's docker container 
https://hub.docker.com/r/yandex/clickhouse-server
3. Use your favourite database conneting tool (Dbeaver for example)
4. Setup connections to local presto and clickhouse instances
5. Insert data from datasets folder to tables
6. Run follow commands to install reqired python packages
```
$
pip install poetry
poetry install
```
7. Open jupyter notebooks from poetry shell
```
$
poetry shell
jupyter notebook guide/0_datasets_check.ipynb
```