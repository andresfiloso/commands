# Postgres

## Connect
```bash
psql -h localhost -p 5432 -U user -d dbname
```

## Introspection
```bash
\l
\dt
\d table
```

## Dump
```bash
pg_dump -h localhost -U user dbname > dump.sql
pg_dump -Fc -h localhost -U user dbname > dump.dump
```

## Restore
```bash
psql -U user -d dbname < dump.sql
pg_restore -U user -d dbname dump.dump
```