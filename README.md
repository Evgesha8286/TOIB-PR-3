# TOIB-PR-3 Pankov Evgeniy Romualdovich BBMO-02-23

1. Создаем 2 виртуальные машины на базе ОС Debian 12 и обеспечиваем между ними сетевой обмен

   ![image](Screenshots/1.png)
   ![image](Screenshots/2.png)
   ![image](Screenshots/3.png)
   
2. Включаем на 1й (сервер) из ВМ передачу логов по протоколу rsyslog на 2ю ВМ (клиент)
   
   **Устанавливаем и настраиваем rsyslog на сервере и клиенте**
   ![image](Screenshots/4.png)

   **Проверяем работоспособность rsyslogна сервере и клиенте**
   ![image](Screenshots/5.png)
   
   **Устанавливаем правила на сервере**
   ![image](Screenshots/6.png)

   **Установка правил на клиент**
   ![image](Screenshots/2.png)

   **Проверка**
   ![image](Screenshots/2.png)

   **Проверка получения логов на сервере**
   ![image](Screenshots/2.png)

6. Установить и настроить получение логов на сервер с использованием Loki
   
 **Установка и редактирование compose-файла на сервере**
 ![image](Screenshots/2.png)
 ![image](Screenshots/2.png)
   
 **Запуск Loki**
 ![image](Screenshots/2.png)

 **Редактирование promtail на клиенте**
 ![image](Screenshots/2.png)

 **Compose-файл для promtail**
 ![image](Screenshots/2.png)

 **Запуск promtail на клиенте**
 ![image](Screenshots/2.png)

 **Просмотр логов клиента в Grafana**
 ![image](Screenshots/2.png)
 
9. Установить и настроить получение логов на сервер с использованием Signoz

   _Установка происходила согласно https://signoz.io/docs/install/docker/#install-signoz-using-docker-compose_

   **Запуск Signoz**
   ![image](Screenshots/2.png)
   ![image](Screenshots/2.png)

   **Редактирование конфигурации на клиенте для отправки данных в Signoz**
   
   _Приложение - https://github.com/SigNoz/sample-nodejs-app/_
   ![image](Screenshots/2.png)

   **Запуск клиентского приложения**
   ![image](Screenshots/2.png)
   
   **Проверка получения логов в Signoz**
   ![image](Screenshots/2.png)
   ![image](Screenshots/2.png)
