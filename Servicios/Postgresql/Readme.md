Para desplegar el siguiente servicio se debe realizar los siguientes pasos:

Para la creacion del imagen
```
docker build -t postgres .
```

Para la creacion del contenedor
```
docker run -d -p 5432:5432 --name postgres_db -v ./postgres_storage:/var/lib/postgresql/data postgres
```