# 1.1

```bash
$ docker ps -a
CONTAINER ID   IMAGE     COMMAND                  CREATED         STATUS                     PORTS     NAMES
3633e2e89e7f   nginx     "/docker-entrypoint.…"   7 minutes ago   Up 7 minutes               80/tcp    condescending_wescoff
57b6ae7f3ad3   nginx     "/docker-entrypoint.…"   7 minutes ago   Exited (0) 7 minutes ago             elated_zhukovsky
1d255b80cfae   nginx     "/docker-entrypoint.…"   7 minutes ago   Exited (0) 7 minutes ago             sleepy_dewdney
```

# 1.2

```bash
$ docker ps -a
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
$ docker images
REPOSITORY   TAG       IMAGE ID   CREATED   SIZE
pena@webserver:~$ exit
```

# 1.3

```bash
$ docker run -it devopsdockeruh/pull_exercise
Give me the password: basics
You found the correct password. Secret message is:
"This is the secret message"
```

# 1.4

```bash
pena@webserver:~$ docker run -d -it --name test devopsdockeruh/exec_bash_exercise
pena@webserver:~$ docker exec -it test bash
root@252dd085616a:/usr/app# tail -f ./logs.txt
"Docker is easy"
```

# 1.5
```bash
$ docker run -d -it --name curler ubuntu:16.04
$ docker exec -it curler bash
# apt update
# apt install curl -y
# exit
$ docker exec -it curler sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
Input website:
helsinki.fi
Searching..
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>301 Moved Permanently</title>
</head><body>
<h1>Moved Permanently</h1>
<p>The document has moved <a href="http://www.helsinki.fi/">here</a>.</p>
</body></html>
```

# 1.6

[Dockerfile](/part1/Dockerfiles/1.6_Dockerfile)

```bash
$ docker run -it docker-clock
1
2
3
4
```

# 1.7

[Dockerfile](/part1/Dockerfiles/1.7_Dockerfile)

```bash
$ docker run --rm -it curler
Input website:
helsinki.fi
Searching..
<!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
<html><head>
<title>301 Moved Permanently</title>
</head><body>
<h1>Moved Permanently</h1>
<p>The document has moved <a href="http://www.helsinki.fi/">here</a>.</p>
</body></html>
```

# 1.8

```bash
$ docker run -v "/usr/app/logs.txt:/usr/app/logs.txt" -d -it devopsdockeruh/first_volume_exercise
```

# 1.9

```console
$ docker run -d --name http -p 5000:80 devopsdockeruh/ports_exercise
$ curl localhost:5000
Ports configured correctly!!
```

# 1.10

[Dockerfile](/part1/Dockerfiles/1.10_Dockerfile)

# 1.11

[Dockerfile](/part1/Dockerfiles/1.11_Dockerfile)

```bash
$ docker run -d --name backend -v "/usr/app/logs.txt:/backend/logs.txt" -p 8000:8000 backend
```

# 1.12

### Frontend

[Dockerfile](/part1/Dockerfiles/1.12_frontend_Dockerfile)

```bash
$ docker run -d --name frontend -p 5000:5000 frontend 
```
[Dockerfile](/part1/Dockerfiles/1.12_backend_Dockerfile)


### Backend
```bash
$ docker run -d --name backend -p 8000:8000 backend
```

# 1.13

[Dockerfile](/part1/Dockerfiles/1.13_Dockerfile)

```bash
$ docker run -d --name java-app -p 8080:8080 java
```

# 1.14


