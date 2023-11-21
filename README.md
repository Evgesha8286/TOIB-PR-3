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
   
   **Установливаем и редактируем compose-файл на сервере**
 
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

   ![image](Screenshots/18.png)
 
 4. Устанавливаем и настроиваем получение логов на сервере с использованием Signoz

   _Установка происходит по инструкции с сайта: https://signoz.io/docs/install/docker/#install-signoz-using-docker-compose_

   **Запускаем Signoz**
   
   ![image](Screenshots/19.png)
   
   ![image](Screenshots/20.png)
   
   ![image](Screenshots/21.png)
   
   **Редактируем конфигурации на клиенте для отправки данных в Signoz**
   
   _Устнаовка приложения согласно инструкции с сайта: https://github.com/SigNoz/sample-nodejs-app/_
   
   ![image](Screenshots/22.png)

   **Запускаем клиентское приложение**
   
   ![image](Screenshots/23.png)
   
   **Проверяем получение логов в Signoz**
   
   ![image](Screenshots/24.png)
   
   ![image](Screenshots/25.png)
