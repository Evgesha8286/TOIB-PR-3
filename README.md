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

   **Включаем UDP и TCP соединение**

   ![image](Screenshots/6.png)

   **Устанавливаем правила на сервере**
   ![image](Screenshots/7.png)

   **Установливаем правила на клиенте**
   
   ![image](Screenshots/8.png)

   **Проверяем получения логов на сервере**
   
   ![image](Screenshots/9.png)

   ![image](Screenshots/10.png)

3. Установить и настроить получение логов на сервер с использованием Loki
   
 **Установливем и редактируем compose-файл на сервере**
 
 ![image](Screenshots/11.png)
 ![image](Screenshots/12.png)
   
 **Запускаем Loki**
 
 ![image](Screenshots/13.png)

 **Редактируем promtail на клиенте**
 
 ![image](Screenshots/14.png)

 **Редактируем compose-файл для promtail**
 
 ![image](Screenshots/15.png)

 **Запускаем promtail на клиенте**
 
 ![image](Screenshots/16.png)

 **Просматриваем логи клиента в Grafana**
 
 ![image](Screenshots/17.png)
 
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
