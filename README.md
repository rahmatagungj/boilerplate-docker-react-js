# boilerplate-docker-react-js
Boiler for basic docer and react js

## Command List
1. Pull NODE JS images
```bash
docker pull node
```

2. Make own react image
```bash
docker build -t react-image .
```

3. Make and Run container with react image
```bash
docker run -d --name react-app -p 3000:3000 -v %cd%\src:/app/src:ro -e CHOKIDAR_USEPOLLING=true react-image
```

### Extra

1. Jump to bash container
```bash
docker exec -it react-app bash
```

2. Kill and remove react-app container
```bash
docker rm react-app -f
```
