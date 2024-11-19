Para desplegar el siguiente servicio se debe realizar los siguientes pasos:

Para la creacion del imagen
```
docker build -t qdrant .
```

Para la creacion del contenedor

Tener en cuenta los siguientes parametros

publicar puertos: -p HOST_PORT:CONTAINER_PORT
```
docker run -d -p 6333:6333 --name qdrant_db -v ./qdrant_data:/qdrant/storage qdrant
```

Para poder entrar al dashboard es con el siguiente enlace

URL: http://localhost:6333/dashboard