# Installation with Docker
You can deploy a localized container of this web app with [Docker](https://www.docker.com/).
1. Clone repository
2. Move into repository directory `cd ./collaborative-planner`
3. Build a Docker image of the app `docker build -t planner .`
4. Run a container with the Docker image `docker run --name myplanner -p 8000:8000 planner`
5. Visit [https://localhost:8000/planner](https://www.docker.com/) to view the app.

# Usage
See the usage of the app in showcase.pdf.