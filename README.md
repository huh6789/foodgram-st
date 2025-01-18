# Запуск

Клонируйте репозиторий:
```bash
git clone https://github.com/huh6789/foodgram-st.git
```
Запуск проекта:
```bash
cd infra
docker-compose up -d
```
Создайте суперпользователя:
```bash
docker-compose exec backend python manage.py createsuperuser
```
Загрузите ингридиенты:
```bash
cd infra
docker-compose exec backend bash
python manage.py load_ingredients data/ingredients.json
```
Доступ к проекту:

Фронтенд доступен по адресу: http://localhost

Тесты проводились в postmen по пути:
postman_collection/foodgram.postman_collection.json
