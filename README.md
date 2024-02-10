# postgresql-backup-restore

```
export POSTGRES_HOST=postgres.domain.com
export POSTGRES_USER=postgres
export POSTGRES_DB=postgres
```

this command backup as dump so you can quikcly restore.

```
pg_dump --format=c $POSTGRES_DB -h $POSTGRES_HOST -U $POSTGRES_USER > survey.dump
```

you can restore different db.

```
pg_restore -h POSTGRES_HOST -p 5432 -U $POSTGRES_USER -d $POSTGRES_DB survey.dump
```
