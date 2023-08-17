# DjangoWeather

### Создание и настройка пользователя\базы 
    sudo -u postgres psql

    psql postgres or sudo -i -u postgres
    
    CREATE DATABASE weather;
    create user user_name_weather with password 'password';
    alter role user_name_weather set client_encoding to 'utf8';
    alter role user_name_weather set default_transaction_isolation to 'read committed';
    alter role user_name_weather set timezone to 'UTC';
    ALTER USER user_name_weather CREATEDB;

    pip3 install -r requirements.txt