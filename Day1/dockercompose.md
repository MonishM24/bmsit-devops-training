# Exercise 5: Docker Compose

## Objective
Run a multi-service stack using Docker Compose.

## What You Will Practice
- Defining multiple services in one file
- Mapping ports
- Setting environment variables
- Starting services together

## Create `docker-compose.yml`
```yaml
version: '3'
services:
  web:
    image: nginx
    ports:
      - "8080:80"

  db:
    image: mysql
    environment:
      MYSQL_ROOT_PASSWORD: root
```

## Run the Stack
```bash
docker-compose up
```

## Notes
- Use `docker-compose up -d` to run in detached mode.
- Stop services with `docker-compose down`.
