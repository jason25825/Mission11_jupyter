mkdir jupyter

cd jupyter

touch docker-compose.yml

version: '3'
services:
  mission11:
    image: jupyter/base-notebook
    container_name: mission11-jupyter-notebook
    ports:
      - "9999:8888"
    volumes:
      - ~/jupyter:/home/jovyan/work


./start.sh
