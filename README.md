Project structure:
```
.
├── docker-compose.yml
├── app
    ├── Dockerfile
    ├── requirements.txt
    └── manage.py


## Deploy with docker compose

```
Let's up docker compose:
```
$ docker compose up -d
```
Check container
```
docker ps
CONTAINER ID   IMAGE        COMMAND                  CREATED          STATUS          PORTS                                       NAMES
e2b2307ef01a   django-web   "python manage.py ru…"   19 minutes ago   Up 19 minutes   0.0.0.0:8000->8000/tcp, :::8000->8000/tcp   django-web-1

```

After the application starts, navigate to `http://localhost:8000` in your web browser:
Output:
![image](https://github.com/joykumarcse/django/assets/99878079/64d97eff-857e-4777-ad0a-28d3f1105e46)


Stop and remove the containers
```
$ docker compose down
```
