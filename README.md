# Contenido

En este repositorio vamos a:

  1. Entrenar un modelo de sklearn
  
  2. Exportarlo usando pickle
  
  3. Construir una API con FastAPI
  
  4. Desplegar la API usando un contendor de Docker

Basado en [FastAPI and Scikit-Learn: Easily Deploy Models](https://nickc1.github.io/api,/scikit-learn/2019/01/10/scikit-fastapi.html)

# Requisitos

 * Python 3.6+

 * Librerías `numpy`, `scikit-learn`, `fastapi`, `uvicorn` y `requests`

 * [Docker](https://docs.docker.com/get-docker/) 

# Instrucciones

```
git clone https://github.com/albertotb/sklearn_fastapi_docker.git
cd sklearn_fastapi_docker
docker build -t api_test .
docker run -d --name api_docker -p 8000:80 api_test
```

# Ejercutar FastAPI

`uvicorn main:app --reload`

# Referencias

 * [Introducción a Docker](https://docs.docker.com/get-started/)
 * [FastAPI and Scikit-Learn: Easily Deploy Models](https://nickc1.github.io/api,/scikit-learn/2019/01/10/scikit-fastapi.html)
 * [FastAPI. Deployment](https://fastapi.tiangolo.com/deployment/)
 * [FastAPI. Imágenes de Docker oficiales](https://github.com/tiangolo/uvicorn-gunicorn-fastapi-docker)
