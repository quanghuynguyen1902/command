# command
Note the command from my experiences


### Docker

- Buid docker images
```javascript
docker build -t "your name of image" . 
```
- List images
```javascript
docker images 
```
- Remove images
```javascript
docker rmi "image_id" or docker rmi -f "ịmage_id" 
```
- Up container 
```javascript
docker-compose up -d 
```
- Down container
```javascript
docker-compose down 
```
- Restart only container
```javascript
docker-compose restart "container_name"
```
- List container
```javascript
docker ps
```
- Logs container
```javascript
docker-compose logs -f "container_id"
```
- Execute container
```javascript
docker-compose exec -it "container_id" bash
```
- List network
```javascript
docker network ls
```
- Check ip address container
```javascript
docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' "container_id"
```
- Check ip address network
```javascript
docker network inspect -f '{{range .IPAM.Config}}{{.Subnet}}{{end}}'  "network_id"
```

