# Hasker

### Учебный сервис вопросов и ответов для самых обездоленных

Разверстка: 
1. создается контейнер с маппингом 80 порта контейнера на 8000 хоста: 
```shell
docker run --rm -it -p 8000:80 ubuntu:latest /bin/bash
```
2. клонируется репозиторий 
```shell
apt update && apt install -y git
git clone https://github.com/pmshoot/hasker /hasker
```
3. заходим в директорию проекта 
```shell
cd /hasker
```
4. собираем и запускаем проект
```shell
apt install -y make
make prod
``` 

Тестовый сервис доступен на порту 8000 