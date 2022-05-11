FROM python:3.9-alpine

WORKDIR /dj_app

COPY ./dj_app /dj_app

RUN pip install -r /dj_app/requirements.txt

RUN python manage.py migrate

EXPOSE 8000

CMD ["python", "/stocks_products/manage.py", "runserver", "0.0.0.0:8000"]
