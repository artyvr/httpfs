# httpfs

A very, very simple file server, distributes files from a directory via **HTTP** (nginx alpine)

Run with `docker-compose.yml`

```yaml
services:
  httpfs:
    image: artyvr/httpfs:latest
    container_name: httpfs
    volumes:
      - ./static:/var/www/static
      - ./images:/var/www/images #optional
      - ./icons:/var/www/icons #optional
      - ./videos:/var/www/videos #optional
      - ./audio:/var/www/audio #optional
    restart: unless-stopped
    ports:
      - 8080:8080
```