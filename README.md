# postgresql-backup-restore

backup

```
pg_dump -h <DB URL> -U <USER> -d <DATABASE> -F c -f backup.dump
```

restore

```
pg_restore -U <USER> -d <DATABASE> backup.dump
```
