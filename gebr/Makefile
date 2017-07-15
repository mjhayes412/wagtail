all:    clean install migrations migrate static

install:
	pip install -r requirements.txt
migrations:
	python manage.py makemigrations
migrate:
	python manage.py migrate
static:
	python manage.py collectstatic --noinput
serve:
	python manage.py runserver
clean:
	find . -type f -name '*.pyc' -delete && find . -type d -name '__pycache__' -delete
shell:
	python manage.py shell
