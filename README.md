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

Migration logs

```bash
Database: jdbc:mysql://db:3306/demodb (MySQL 5.7)
MySQL 5.7 is outside of Redgate community support. See https://rd.gt/468B6ni for details
Schema history table `demodb`.`flyway_schema_history` does not exist yet
Successfully validated 2 migrations (execution time 00:00.018s)
Creating Schema History table `demodb`.`flyway_schema_history` ...
Current version of schema `demodb`: << Empty Schema >>
Migrating schema `demodb` to version "1 - create user table"
Migrating schema `demodb` to version "2 - create test user"
Successfully applied 2 migrations to schema `demodb`, now at version v2 (execution time 00:00.087s)
```

Check your user table

![Captura de tela 2024-11-03 014634](https://github.com/user-attachments/assets/7a82b1fd-4261-4a97-8830-6cf538648044)

Success! ✅
