```
docker build -t open-webui .
```

```
docker run -d -p 3000:8080 --add-host=host.docker.internal:host-gateway -v ./open-webui:/app/backend/data --name open-webui-web --restart always open-webui
```