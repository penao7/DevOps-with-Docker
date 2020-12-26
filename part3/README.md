
# [Part 3](https://devopswithdocker.com/part3/)

## 3.1

## Before

```bash
$ docker images
REPOSITORY   TAG          IMAGE ID       CREATED         SIZE
frontend     latest       1297a69cdece   13 minutes ago  778MB
backend      latest       9faa2dfe7375   26 minutes ago  522MB
```

## After 

```bash
$ docker images
REPOSITORY   TAG          IMAGE ID       CREATED          SIZE
frontend     latest       500b3a8f9040   8 seconds ago    494MB
backend      latest       a12bc1808f05   16 seconds ago   299MB
```

## 3.2 Deployment pipeline to heroku

[buttongame-pipeline](https://github.com/penao7/buttongame-pipeline)

## 3.3 Building images inside of a container

[imagebuilder](https://github.com/penao7/docker-imagebuilder)


