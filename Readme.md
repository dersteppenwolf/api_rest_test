# Publicación de servicio REST con Python



https://fastapi.tiangolo.com/deployment/docker/

https://fastapi.tiangolo.com/deployment/docker/#official-docker-image-with-gunicorn-uvicorn

https://fastapi.tiangolo.com/deployment/docker/#build-a-docker-image-for-fastapi


```bash

cd C:\opt\work\igac\git\api_rest_test


docker build -t derstepp/api_rest_test .

docker rm -f api_rest_test 

docker run -d --name api_rest_test -p 80:80 derstepp/api_rest_test:latest


docker logs -f api_rest_test


http://localhost/items/5?q=somequery
http://localhost/docs
http://localhost/redoc
http://localhost/openapi.json



```