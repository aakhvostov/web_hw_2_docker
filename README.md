# Домашнее задание к лекции «Docker»

## Задание 1

По аналогии с практикой из лекции создайте свой docker image с http сервером nginx. Замените страницу приветсвия Nginx на своё (измените текст приветствия на той же странице).

Для создания образа выполнить:

docker build --tag netology:1.0 .


## Задание 2

Создайте контейнер для REST API сервера из решения ДЗ по теме «Flask»

1. Создайте типовой Docker-файл для запуска Python-приложения
2. Проверьте конфигурацию Flask на использование переменных окружения (environment)
3. Проверьте Docker-файл на передачу переменных окружения в Flask
4. Docker-контейнер запускается с приложением Flask

Для создания образа выполнить:

docker build --tag netology:2.0 .

### Типовые команды для запуска контейнера:

Для создания контейнера выполнить команды:

1. docker container run --rm -dt --name nginx netology:1.0
или 
1. docker container run --rm -dt --name flask netology:2.0

Для остановки контейнера выполнить команды:

2. docker container stop nginx
или 
2. docker container stop flask

Для подключения к контейнеру выполнить команды:

3. docker container exec -it nginx bash
или 
3. docker container stop -it flask python