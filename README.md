En este repositorio vamos a:

  1. Entrenar un modelo de sklearn
  
  2. Exportarlo usando pickle
  
  3. Construir una API con FastAPI
  
  4. Desplegar la API usando un contendor de Docker

# Instrucciones

```
git clone https://github.com/albertotb/sklearn_fastapi_docker.git
cd sklearn_fastapi_docker
docker build -t myapi .
docker run -d --name myapicontainer -p 80:80 myapi
```

# Referencias

 * [FastAPI and Scikit-Learn: Easily Deploy Models](https://nickc1.github.io/api,/scikit-learn/2019/01/10/scikit-fastapi.html)
 * [FastAPI. Deployment](https://fastapi.tiangolo.com/deployment/)
 * [FastAPI. Imágenes de Docker oficiales](https://github.com/tiangolo/uvicorn-gunicorn-fastapi-docker)
