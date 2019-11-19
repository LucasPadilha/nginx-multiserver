# README for Nginx proxy


1. Create docker network
```bash
	docker network create nginx-proxy
```

2. Run nginx proxy container
```bash
	docker-compose -f docker-compose.yml up -d 
```

3. Run any application container you want, just remember to set the environment variables (like the example above)
```bash
	docker-compose -f docker-compose-apache.yml build
	docker-compose -f docker-compose-apache.yml up -d 
```