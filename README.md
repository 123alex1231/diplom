# Дипломная работа «Облачное хранилище»
## Описание проекта
Задача — разработать REST-сервис. Сервис должен предоставить REST-интерфейс для загрузки файлов и вывода списка уже загруженных файлов пользователя. Все запросы к сервису должны быть авторизованы. Заранее подготовленное веб-приложение (FRONT) должно подключаться к разработанному сервису без доработок, а также использовать функционал FRONT для авторизации, загрузки и вывода списка файлов пользователя.

## Реализация
Приложение разработано с использованием Spring Boot
Использован сборщик пакетов maven
Для запуска используется docker, docker-compose
Код размещен на github
Код покрыт unit тестами с использованием mockito
Добавлены интеграционные тесты с использованием testcontainers
## Описание и запуск FRONT
Установите nodejs (версия не ниже 19.7.0) на компьютер, следуя инструкции https://nodejs.org/ru/download/current.
Скачайте FRONT https://github.com/netology-code/jd-homeworks/tree/master/diploma/netology-diplom-frontend (JavaScript).
Перейдите в папку FRONT приложения и все команды для запуска выполняйте из неё.
Следуя описанию README.md FRONT проекта, запустите nodejs-приложение (npm install, npm run serve).
Далее нужно задать url для вызова своего backend-сервиса.
В файле .env FRONT (находится в корне проекта) приложения нужно изменить url до backend, например: VUE_APP_BASE_URL=http://localhost:8080.
Нужно указать корневой url вашего backend, к нему frontend будет добавлять все пути согласно спецификации
Для VUE_APP_BASE_URL=http://localhost:8080 при выполнении логина frontend вызовет http://localhost:8080/login
Запустите FRONT снова: npm run serve.
Изменённый url сохранится для следующих запусков.
По умолчанию FRONT запускается на порту 8080 и доступен по url в браузере http://localhost:8080.
Если порт 8080 занят, FRONT займёт следующий доступный (8081). После выполнения npm run serve в терминале вы увидите, на каком порту он запустился.
