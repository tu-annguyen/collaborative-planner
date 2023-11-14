# Installation
1. Install [py4web](https://github.com/web2py/py4web)
2. Clone this repository
3. Move into repository directory `cd ./collaborative-planner`
4. Run the app with `python <path-to-py4web.py> run apps`
5. Visit [https://localhost:8000/planner](https://localhost:8000/planner) to view the app.
## Using Docker
You can deploy a localized container of this web app with [Docker](https://www.docker.com/).
Make sure you are in the root directory for this repository.
1. Build a Docker image of the app `docker build -t planner .`
2. Run a container with the Docker image `docker run --name myplanner -p 8000:8000 planner`
3. Visit [https://localhost:8000/planner](https://localhost:8000/planner) to view the app.

# Usage
See the usage of the app in showcase.pdf.