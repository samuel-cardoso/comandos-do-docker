# comandos-do-docker

O comando mais comum para iniciar os containers do Docker definidos em um arquivo `docker-compose.yml` é:

```bash
docker-compose up
```

Se você quiser iniciar os containers em segundo plano (modo **detached**), use:

```bash
docker-compose up -d
```

> ⚠️ Em versões mais recentes do Docker, o comando recomendado é `docker compose` (sem o hífen), então os equivalentes seriam:

```bash
docker compose up
```

e

```bash
docker compose up -d
```

### Outros comandos úteis:

* **Parar os containers:**

  ```bash
  docker compose down
  ```

* **Recriar containers sem cache:**

  ```bash
  docker compose up --build
  ```

Se quiser iniciar containers individuais (sem `docker-compose`), o comando seria:

```bash
docker start <nome_do_container>
```

E para listar todos os containers (mesmo os parados):

```bash
docker ps -a
```
