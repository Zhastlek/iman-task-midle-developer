# iman-task-middle-developer

### Тестирование программы:
- Открываем postman и выбираем заранее созданную коллекцию для теста. Ссылка на коллекцию в postman: https://go.postman.co/workspace/Team-Workspace~d861f7b1-f86b-41dc-8392-4f629e35c170/collection/20613327-606e7515-29ce-43c8-b485-2b5f24067bd5?action=share&creator=20613327 
- Все методы и способы предачи данных созданы в данной колекции

### Запуск программы:
1. Запускаем базу данных PostgreSql: пишем в терминале **make docker**
2. Запускаем микросервисы: открываем второй терминал и пишем **make run**
3. После работы с программой удаляем образ PostgreSql: пишем **make clean**

## Тестовое задание

**Необходимо создать маленькое микросервисное приложение, состоящее из 3 микросервисов**
### Сервис №1
- Задача сервиса собрать 50 страниц постов из открытого API - https://gorest.co.in/public/v1/posts
- Собранные данные необходимо сохранить в ДБ (Любую на выбор).
* Будет плюсом если данные будут собираться в несколько потоков.
### Сервис №2
Сервис должен реализовать логику GRUD для собранных ранее постов:
- Возможность получить несколько постов.
- Возможность получить конкретный пост
- Возможность удалить пост
- Возможность изменить пост
### Сервис №3
Сервис должен являться API Gateway (REST API) и предоставить методы для выполнения операций сервиса №1 и сервиса №2.  
- Запуск процесса сбора данных и возможности проверки окончания процесса
- Методы GRUD сервиса №2

***Взаимодействие между сервисами должно осуществляться по gRPC.***
Задание нужно расположить в любом Git репозитории и предоставить ссылку.
