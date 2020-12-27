
# [Part 3](https://devopswithdocker.com/part3/)

## 3.1

## Before optimization

```bash
$ docker images
REPOSITORY   TAG          IMAGE ID       CREATED         SIZE
frontend     latest       1297a69cdece   13 minutes ago  778MB
backend      latest       9faa2dfe7375   26 minutes ago  522MB
```

## After optimization

```bash
$ docker images
REPOSITORY   TAG          IMAGE ID       CREATED          SIZE
frontend     latest       500b3a8f9040   8 seconds ago    494MB
backend      latest       a12bc1808f05   16 seconds ago   299MB
```

## 3.2 Deployment pipeline to heroku

[buttongame-pipeline-github](https://github.com/penao7/buttongame-pipeline)

## 3.3 Building images inside of a container

[imagebuilder-github](https://github.com/penao7/docker-imagebuilder)

## 3.4 

[frontend_dockerfile](/part3/Dockerfiles/3.4_Dockerfile_frontend)

[backend_dockerfile](/part3/Dockerfiles/3.4_Dockerfile_backend)

## 3.5

#### Before optimization

```bash
REPOSITORY     TAG          IMAGE ID       CREATED          SIZE
backend        latest       086a4f0bdc3c   7 minutes ago    300MB
frontend       latest       0426954ee14b   13 minutes ago   495MB
```

#### After optimization

[frontend_dockerfile](/part3/Dockerfiles/3.5_Dockerfile_frontend)

[backend_dockerfile](/part3/Dockerfiles/3.5_Dockerfile_backend)


```bash
REPOSITORY     TAG          IMAGE ID       CREATED         SIZE
backend        latest       089b0560d6fa   2 minutes ago   129MB
frontend       latest       f2a99eaf4df4   8 minutes ago   328MB
```

## 3.6

[frontend_dockerfile](/part3/Dockerfiles/3.6_Dockerfile_frontend)

## 3.7

[imagebuilder_dockerfile_before](/part3/Dockerfiles/3.7_Dockerfile_imagebuilder_before)

[imagebuilder_dockerfile_after](/part3/Dockerfiles/3.7_Dockerfile_imagebuilder_after)

## 3.8

picture doesnt look like it should when using dark mode

![kubernetes](/part3/images/kubernetes.png)
