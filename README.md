# News DB

![Deploy DB](https://github.com/c8112002/news-db/workflows/Deploy%20DB/badge.svg)

## Getting started

### dev

start up DB

```bash
docker-compose up -d
```

```bash
./bin/dev.sh migrate! up
./bin/dev.sh migrate! down
```

seeding

```bash
./bin/dev.sh seed
```

reset

```bash
./bin/dev.sh reset
```


### production

Set environment variables.
```bash
export rMYSQL_DATABASE=***
export rMYSQL_USER=***
export rMYSQL_PASSWORD=***
export rMYSQL_ROOT_PASSWORD=***
```

start up DB

```bash
docker-compose -f docker-compose_prod.yaml run --service-ports -d db 
```

migration

```bash
./bin/prod.sh migrate! up
./bin/prod.sh migrate! down
```

seeding

```bash
./bin/prod.sh seed
```

reset

```bash
./bin/prod.sh reset
```
