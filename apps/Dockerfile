# FROM python:3.7.5
# WORKDIR /collaborative-planner
# RUN python -m pip install --upgrade pip && python -m pip install --upgrade py4web
# COPY . ./apps
# RUN py4web set_password --password "mypassword"
# CMD ["py4web", "run", "apps"]

FROM ubuntu:latest

RUN apt update && \
    apt install -y git python3 python3-pip memcached && \
    service memcached restart && \
    python3 -m pip install -U py4web

WORKDIR /collaborative-planner

COPY . ./apps

RUN py4web set_password --password "mypassword"

CMD py4web run --password_file password.txt --host 0.0.0.0 --port 8000 apps