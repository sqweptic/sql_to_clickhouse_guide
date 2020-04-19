SQL syntax queries to clickhouse systax queries guide

Example tables description:

Users
id
firstname
lastname
nickname


Notifications
id
user_id
email
push_android
push_ios
sms


Transactions
id
user_id
transaction_time
transaction_date
revenue
currency_id
currency_ratio
is_acceptable
refund_time
refund_date


Visits
visit_id
visit_time
visit_date
user_id
page_name


Calendar
dt

Try:
Easiest way to try translate some sql query to clickhouse query.
1. Use docker classic sql syntax db (presto for example) https://hub.docker.com/r/prestosql/presto
2. Use docker clickhouse https://hub.docker.com/r/yandex/clickhouse-server
3. Use your favourite db connetion utility (Dbeaver for example)
4. Setup connection to local presto and clickhouse servers