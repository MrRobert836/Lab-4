# Лабораторная работа №4

## Цель работы

Сделать мониторинг сервиса с помощью prometheus и grafana

## Ход работы

Установка Prometheus:

<p align="center">
    <img src="./img/image-1.png">
</p>

Запуск сервисов Prometheus:

<p align="center">
    <img src="./img/image-2.png">
</p>

Установка Grafana:

<p align="center">
    <img src="./img/image-3.png">
</p>

Запуск сервисов Grafana:

<p align="center">
    <img src="./img/image-4.png">
</p>


С помощью команды `kubectl get all` было проверна работовпособность сервисов.

<p align="center">
    <img src="./img/image-5.png">
</p>

Запуск Prometheus:
<p align="center">
    <img src="./img/image-6.png">
</p>

После запуска открылась страница в браузере:

<p align="center">
    <img src="./img/image-7.png">
</p>

Запуск Grafana:

<p align="center">
    <img src="./img/image-8.png">
</p>

Для того, чтобы войти в сервис Grafana нужно ввести логин, в нашем случае: `admin` и пароль, который был расшифрован и записан в файлик с помощью следующих команд:

<p align="center">
    <img src="./img/image-9.png">
</p>

После введения логина и пароля открылась страница Grafana в браузере:

<p align="center">
    <img src="./img/image-10.png">
</p>

После было настроено получение Grafana метрик с Prometheus. Для этого перешли в раздел Data sourses создан новый Dashboard


















