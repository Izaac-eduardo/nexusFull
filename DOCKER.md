# Docker - Nexus

Execute na raiz do projeto.

## Primeiro uso

```bash
cp .env.example .env
```

Edite `.env` e troque `DB_USER`, `DB_PASSWORD`, `DB_ROOT_PASSWORD` e `JWT_SECRET`.

## Subir tudo

```bash
docker compose up -d --build
```

Aplicacao:

```text
http://localhost:8080
```

API direta:

```text
http://localhost:3000/health
```

MySQL no host:

```text
localhost:3307
```

Dentro do Docker, backend usa:

```text
db:3306
```

## Comandos uteis

```bash
docker compose ps
docker compose logs -f backend
docker compose logs -f db
docker compose logs -f frontend
docker compose stop
```

## Limpar containers

```bash
docker compose down
```

## Limpar containers e dados do MySQL

```bash
docker compose down -v
```
