# Django docker
[from tutorial](https://blog.devartis.com/django-development-environment-with-docker-a-step-by-step-guide-ae234612fa61)

## Installation

```bash
mkvirtualenv MYPROJECT_NAME
git clone PROJECT_URL
pip install -r requirements.txt
docker-compose up -d
python manage.py collectstatic
python manage.py migrate
docker-compose stop
docker-compose start
python manage.py runserver 0.0.0.0:8001
```
Open [localhost](http://localhost/) in your browser *I STRONGLY RECOMEND FIREFOX* 

## Commands

create & start containers
```
docker-compose up 
```
stop containers without losing migrations (db persistanca)
```
docker compose stop
```
