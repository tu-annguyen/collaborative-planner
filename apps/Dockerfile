FROM python:3.7.5
WORKDIR /collaborative-planner
RUN python -m pip install --upgrade pip && python -m pip install --upgrade py4web
COPY . ./apps
RUN py4web set_password --password "mypassword"
CMD ["py4web", "run", "apps"]