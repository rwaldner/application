
# Simple JAR File with minimal Java output

## Build
```
cd ~/Workspaces/application
./gradlew jar
```

## Run
### Directly on the command line
```
cd ~/Workspaces/application
java -cp build/libs/application.jar Main
```

### Using gradle
```
cd ~/Workspaces/application
./gradlew run
```

## Run in Docker Container
```
cd ~/Workspaces/application
docker run -v `pwd`:/tmp -it --rm openjdk:8u151-jre-alpine3.7 "/tmp/docker-run.sh"
```
