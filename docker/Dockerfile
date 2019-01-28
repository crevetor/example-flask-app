FROM tiangolo/uwsgi-nginx:python3.6

RUN pip install pipenv --upgrade
ADD Pipfile* /app/
RUN pipenv install --system

ADD docker/uwsgi.ini /app
COPY ./src /app
