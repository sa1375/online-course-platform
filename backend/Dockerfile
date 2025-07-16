# latest official Python image
FROM python:3.12-slim

# set workdir
WORKDIR /app

# copy source code
COPY . /app

# install pip and dependencies
RUN pip install --upgrade pip && \
    pip install django djangorestframework psycopg2-binary

EXPOSE 8000

# run development server
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]