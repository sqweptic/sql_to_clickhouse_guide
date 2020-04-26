## Guide to converting SQL queries to clickhouse systax queries (which pseudo-sql)

Clickhouse queries syntax is quite unusual compared to regular sql. (sql-92 / sql-03 and so on).
So here is the guide for.

#### Datasets source
1. bank accounts dataset - [Kaggle](https://www.kaggle.com/apoorvwatsky/bank-transaction-data)

#### Try
Easiest way to try examples from here is follow: 
1. Use docker classic sql syntax db (presto for example) https://hub.docker.com/r/prestosql/presto
2. Use docker clickhouse https://hub.docker.com/r/yandex/clickhouse-server
3. Use your favourite database conneting tool (Dbeaver for example)
4. Setup connection to local presto and clickhouse servers
5. Insert data from datasets folder to tables
6. Run commands to install reqired packages
install python
curl https://pyenv.run | bash
pip install poetry
7. Go to guide to try