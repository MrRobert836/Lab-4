# Лабораторная работа №4

## Цель работы

Сделать мониторинг сервиса с помощью prometheus и grafana

## Ход работы

Установка Prometheus:

<p align="center">
    <img src="./images/image-1.png">
</p>

Запуск сервисов Prometheus:

<p align="center">
    <img src="./images/image-2.png">
</p>

Установка Grafana:

<p align="center">
    <img src="./images/image-3.png">
</p>

Запуск сервисов Grafana:

<p align="center">
    <img src="./images/image-4.png">
</p>


С помощью команды `kubectl get all` была проверена работоспособность сервисов.

<p align="center">
    <img src="./images/image-5.png">
</p>

Запуск Prometheus:
<p align="center">
    <img src="./images/image-6.png">
</p>

После запуска открылась страница в браузере:

<p align="center">
    <img src="./images/image-7.png">
</p>

Запуск Grafana:

<p align="center">
    <img src="./images/image-8.png">
</p>

Для того, чтобы войти в сервис Grafana нужно ввести логин, в нашем случае: `admin` и пароль, который был расшифрован и записан в файлик с помощью следующих команд:

<p align="center">
    <img src="./images/image-9.png">
</p>

После введения логина и пароля открылась страница Grafana в браузере:

<p align="center">
    <img src="./images/image-10.png">
</p>

После было настроено получение Grafana метрик с Prometheus. Для этого в разделе «connection - data source». Было добавлено соединение с Prometheus.

<p align="center">
    <img src="./images/image-11.png">
</p>

После был создан новый Dashboard в качестве типа отображения был импортирован node-exporter-full (по id) на странице, которую рекомендует Grafana (https://grafana.com/grafana/dashboards/)

Результат:

<p align="center">
    <img src="./images/image-12.png">
</p>

## Вывод

Был успешно настроен мониторинг сервиса, запущенного в Kubernetes, с использованием Prometheus и Grafana. Было настроено отображение графиков для отслеживания 
нагрузки
