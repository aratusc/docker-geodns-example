# GeoDNS realization created with PowerDNS and MySQL

## Idea

### We needed a GeoDNS implementation, that could be dynamically modified. By default PowerDNS does'nt support GeoIP with MySQL dynamically in real time.

## Environment variables

- `MYSQL_HOST` database host
- `MYSQL_PORT` database port
- `MYSQL_USER` username
- `MYSQL_PASS` password
- `MYSQL_NAME` database name
- `PDNS_API_KEY` PowerDNS API key
- `PDNS_ADMIN_SECRET` PowerDNS admin secret
- `PDNS_ALLOW_AXFR_IPS` PowerDNS AXFR ip ranges, separated by commas 

## Setup

```
chmod +x ./setup.sh

./setup.sh

docker compose build 

docker compose up -d
```
