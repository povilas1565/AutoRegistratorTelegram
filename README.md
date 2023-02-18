# Automatic Registrator Telegram Accounts.
Автоматический регистратор телеграм аккаунтов.

## Предпосылки:
1) API кода подтверждения телефона. Зарегистрируйте аккаунт на [getsmscode.com](https://www.getsmscode.com/) и пополнить на несколько долларов. 
2) Аккаунт Telegram с *api_id* и *api_hash*. Посетите https://my.telegram.org/apps and заполните там формы.

## Установка:
```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```
## Как пользоваться:
1) Создайте конфигурационный файл с именем *config.ini* в корневом каталоге.

```
touch config.ini
```
2) Добавьте ваше имя пользователя и токен.

> [pyrogram]  
> api_id = YOUR_TELEGRAM_API_ID  
> api_hash = YOUR_TELEGRAM_API_HASH  

> [GetSMSCode.com]  
> username = YOUR_USERNAME  
> token = YOUR_TOKEN  
> api_url = http://www.getsmscode.com/do.php  

3) Запуск
```
python main.py
```

