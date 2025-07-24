FROM clickhouse/clickhouse-server:25.6.2.5-alpine

# from https://github.com/umami-software/umami/blob/master/db/clickhouse/schema.sql
# alternatively, the schema can be manually applied after clickhouse starts
ADD schema.sql /docker-entrypoint-initdb.d/schema.sql

ADD logs.xml /etc/clickhouse-server/config.d/
ADD async-write.xml /etc/clickhouse-server/users.d/
