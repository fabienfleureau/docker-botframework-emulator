# docker-botframework-emulator
Dockerfile for microsoft botframework emulator

### How to run bot framework emulator:

```docker run -i fabienfleureau/botframework-emulator```


#### Usage:

See http://docs.botframework.com/connector/tools/bot-framework-emulator/#mac-and-linux-support-using-command-line-emulator


configure endpoint by typing
```
/settings
```

example endpoint value:

```
http://10.10.10.10:3978/api/messages
```
!!! warning !!! localhost is not valid hostname since emulator run in a private docker network

### Build & run from sources:

build:

```
git pull https://github.com/fabienfleureau/docker-botframework-emulator.git
cd docker-botframework-emulator
docker build -t botframework-emulator .
```

run:

```docker run -i botframework-emulator```
