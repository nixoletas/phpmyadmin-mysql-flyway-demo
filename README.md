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

Check your user table

![Captura de tela 2024-11-03 014634](https://github.com/user-attachments/assets/7a82b1fd-4261-4a97-8830-6cf538648044)

Success! ✅
