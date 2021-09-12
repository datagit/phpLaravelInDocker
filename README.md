#### setup ENV
```bash
# apache2
# php
# php extensions: redis, mongodb, xdebug
# editor: VSCode

docker build -t myphp/7.4-xmr-apache --build-arg USER_ID=$(id -u) --force-rm -f Dockerfile .
docker-compose up -d
docker-compose down
docker exec -it backend bash
```