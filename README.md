# Django_app
# raising the project using Postgres, Gunicorn, and Nginx

# How deploy:
1) add .env.dev; .env.prod; .env.db to source root
2) Run command docker-compose up -d --build and go to http://localhost:8000 (local)
If this pruction
1) docker-compose -f docker-compose.prod.yml up -d --build and go to http://localhost:1337 (production)
2) docker-compose -f docker-compose.prod.yml exec python manage.py migrate
3) docker-compose -f docker-compose.prod.yml exec python manage.py createsuperuser
4) docker-compose -f docker-compose.prod.yml exec python manage.py test
