Run DB and PhpMyAdmin

```bash
docker compose up -d
```

Acess: http://localhost:8090

```
username: demouser
password: password
```

Run migrations

```bash
docker start demo-migrations && docker logs demo-migrations -f
```
