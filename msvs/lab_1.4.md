# ЛР 1.3. Настройка клиента службы DNS

### Задание 1. Настройте клиентскую часть DNS.

1. Запустите виртуальную машину и загрузите ОС Windows. 
2. Откройте окно Сетевые подключения. 
3. Вызовите свойства Подключения по локальной сети (контекстное меню/Свойства). 
4. Вызовите свойства Протокол Интернета TCP/IP. 
5. Установите адреса DNS серверов: 
    - установите переключатель Использовать следующие адреса DNS-серверов; 
    - в поле Предпочитаемый DNS-сервер введите ```172.21.0.1```; 
    - в поле Альтернативный DNS-сервер ведите ```172.21.0.2```. 
6. Добавьте 3-й DNS сервер. Для этого: 
    - щелкните Дополнительно; 
    - перейдите на вкладку DNS; 
    - щелкните Добавить в разделе Адреса DNS-серверов; 
    - введите ```172.21.1.1``` сервера имен и закройте окно кнопкой OK. 
7. Закройте диалоговое окно Свойства: Протокол Интернета TCP/IP кнопкой ОК. 
8. Закройте окно свойств локального подключения. 
9. Закройте окно Сетевые подключения. 
10. Проверьте настройки. Для этого с помощью команды ping отправьте эхо-запросы на символьный адрес компьютера в учебной сети, например server1. Сделайте снимок экрана.

### Задание 2. Настройте компьютер для разрешения имен при отсутствии DNS-сервера.
1. Соберите информацию об адресах компьютеров в кабинете (символьные адреса и IP-адреса). Для этого воспользуйтесь командой ping. 
2. Откройте файл hosts (c:\WINDOWS\system32\drivers\etc\hosts). 
3. Внесите в этот файл собранную информацию о первом компьютере в кабинете, например:
```
172.21.5.32		Computer_1
```
4. Аналогично внесите информацию об остальных компьютерах. 
5. Проверьте внесенные изменения: 
    - удалите в настройках Подключения по локальной сети все записи DNS серверов; 
    - отправьте эхо-запрос на какой-нибудь компьютер по его символьному адресу (если будет получен ответ, то настройки верны)
    - Сделайте снимок экрана.

