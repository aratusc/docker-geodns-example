# GeoDNS realization created with PowerDNS and MySQL

## Idea

### We needed a GeoDNS implementation, that could be dynamically modified. By default PowerDNS does'nt support GeoIP with MySQL dynamically in real time.

## Environment variables

- `MYSQL_HOST` MySQL host
- `MYSQL_PORT` MySQL port
- `MYSQL_USER` MySQL username
- `MYSQL_PASS` MySQL password
- `MYSQL_NAME` MySQL database name
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
