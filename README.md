# 1. Создайте свой кастомный образ nginx на базе alpine. После запуска nginx должен отдавать кастомную страницу (достаточно изменить дефолтную страницу nginx)

Создано два образа, https://hub.docker.com/r/nuteshev/nginx и https://hub.docker.com/r/nuteshev/php-fpm. Для запуска их нужно использовать прилагаемый файл docker-compose.yml, а именно, 
зайти в папку, где он лежит, и набрать команду 

```
docker-compose up -d
```

После этого на 80-м порту машины, где находится Docker, можно будет увидеть кастомную страницу. 

# 2. Определите разницу между контейнером и образом. Вывод опишите в домашнем задании.
Контейнер - это конкретная совокупность процессов, запущенная из образа. Образ является шаблоном для создания контейнеров.  

# 3. Ответьте на вопрос: Можно ли в контейнере собрать ядро?
Нет, т.к. контейнер использует ядро основной системы. 

# 4. Создайте кастомные образы nginx и php, объедините их в docker-compose

См. выше пункт 1. 