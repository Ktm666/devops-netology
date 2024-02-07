1. Задача 1
   Сценарий выполнения задачи:

создайте свой репозиторий на https://hub.docker.com;
выберите любой образ, который содержит веб-сервер Nginx;
создайте свой fork образа;
реализуйте функциональность: запуск веб-сервера в фоне с индекс-страницей, содержащей HTML-код ниже:
<html>
<head>
Hey, Netology
</head>
<body>
<h1>I’m DevOps Engineer!</h1>
</body>
</html>
Опубликуйте созданный fork в своём репозитории и предоставьте ответ в виде ссылки на 
https://hub.docker.com/repository/docker/ktm6/nginx/general
docker push ktm6/nginx:1.0


2. Посмотрите на сценарий ниже и ответьте на вопрос: «Подходит ли в этом сценарии использование Docker-контейнеров или лучше подойдёт виртуальная машина, физическая машина? Может быть, возможны разные варианты?»
Детально опишите и обоснуйте свой выбор.
Сценарий:
высоконагруженное монолитное Java веб-приложение;
Nodejs веб-приложение;
мобильное приложение c версиями для Android и iOS;
шина данных на базе Apache Kafka;
Elasticsearch-кластер для реализации логирования продуктивного веб-приложения — три ноды elasticsearch, два logstash и две ноды kibana;
мониторинг-стек на базе Prometheus и Grafana;
MongoDB как основное хранилище данных для Java-приложения;
Gitlab-сервер для реализации CI/CD-процессов и приватный (закрытый) Docker Registry.

 Ответ
    1. Для более простой миграции приложения можно использовать докер с образом JVM или ВМ, а так же я считаю, что для данного видо приложения подойдет физический сервер, так как это монолит
    2. Контейнер, так как снижает трудозатраты и развертывание приложений
    3. Физический сервер или ВМ, так как контейнеризация не подходит для работы с UI
    4. Лучше всего подойдет размещение на ВМ исходя из документации Apache Kafka
    5. Контейнеризация, так как все приложения для Elasticsearch будут работать в контенерах докер и занимать меньше ресурсов, работая на однйо ВМ
    6. Для облегчения развертывания и масшатабирования можно использовать контейнерезацию или ВМ
    7. Возможно использовать все три варианты, но при использовании контейнерезации необходимо выносить отдельный том для хранения данных
    8. Исходя из документации может быть размещен в всех трех вариантах


4. Воспроизведите практическую часть лекции самостоятельно.
Соберите Docker-образ с Ansible, загрузите на Docker Hub и пришлите ссылку вместе с остальными ответами к задачам.

https://hub.docker.com/repository/docker/ktm6/ansible/general
docker push ktm6/ansible:2.9.1