# News DB

![Deploy DB](https://github.com/c8112002/news-db/workflows/Deploy%20DB/badge.svg)

## Getting started

### dev

migration

```bash
docker-compose up -d
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

