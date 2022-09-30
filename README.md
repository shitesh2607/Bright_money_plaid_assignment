# Bright_money_plaid_assignment

## Set up

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
