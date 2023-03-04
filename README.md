## Daniel Tegenrot portfolio

Based on https://github.com/docker/awesome-compose/tree/master/django

## Deploy with docker compose

```
docker compose up -d --build web

```

## Expected result

Listing containers must show one container running and the port mapping as below:
```
$ docker ps
CONTAINER ID        IMAGE               COMMAND                  CREATED              STATUS              PORTS                    NAMES
3adaea94142d        django_web          "python3 manage.py r…"   About a minute ago   Up About a minute   0.0.0.0:8000->8000/tcp   django_web_1
```

After the application starts, navigate to `http://localhost:8000` in your web browser:

Stop and remove the containers
```
$ docker compose down
```
