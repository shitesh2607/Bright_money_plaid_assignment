# Bright_money_plaid_assignment

## Set up
##### Note: create enviroment variable to isolate the app and better experience.

### Install Dependencies
```bash
--- pip install -r requirements.txt 
```
### Install RabbitMQ Celery Broker
```bash
--- sudo apt-get install rabbitmq-server (Ubuntu)
```

### Enable RabbitMQ server

```bash
--- systemctl enable rabbitmq-server
```

### Start RabbitMQ server

```bash
--- systemctl start rabbitmq-server
```
### Create and Apply Migrations
```bash
--- python manage.py makemigrations
--- python manage.py migrate
```

### Start Celery Worker Process
```bash
--- celery -A Bright_money_plaid_assignment worker -l info
```

### Start Your Django App
```bash
--- python manage.py runserver
```
### API's Endpoint
![path](https://user-images.githubusercontent.com/72928430/193238242-8b86be96-48ad-411f-8a00-26598eb0c463.png)

