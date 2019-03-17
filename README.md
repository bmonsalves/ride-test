

## Development

construir imagenes y levantar imagenes
```bash
docker-compose -f local.yml build
docker-compose -f local.yml up
```

Estado de los contenedores
```bash
docker-compose -f local.yml ps
```

evitar agregar -f local.yml a los comandos
```bash
export COMPOSE_FILE=local.yml
docker-compose up
docker-compose down
```

correr contenedor de django por separado
```bash
docker rm -f CONTAINER
docker-compose run --rm --service-ports django

```

comandos de administracion
```bash
docker-compose run --rm django python3 manage.py COMMAND
```

