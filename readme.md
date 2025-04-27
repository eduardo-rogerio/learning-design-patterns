
Instala o projeto
```bash
 docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v "$(pwd):/var/www" \
    -w /var/www \
    composer:latest \
    composer install --ignore-platform-reqs
```

Atualiza o projeto
```bash
 docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v "$(pwd):/var/www" \
    -w /var/www \
    composer:latest \
    composer update --ignore-platform-reqs
```
Abre um terminal. 
```bash
docker compose exec php sh
```
