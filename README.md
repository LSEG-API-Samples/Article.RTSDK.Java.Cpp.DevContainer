## Try Examples
https://github.com/microsoft/vscode-remote-try-java
https://github.com/microsoft/vscode-remote-try-node

## Resources
https://code.visualstudio.com/docs/remote/containers-tutorial
https://code.visualstudio.com/docs/remote/containers
https://code.visualstudio.com/docs/remote/attach-container
https://code.visualstudio.com/remote/advancedcontainers/develop-remote-host
https://code.visualstudio.com/docs/remote/create-dev-container#_set-up-a-folder-to-run-in-a-container
https://code.visualstudio.com/remote/advancedcontainers/develop-remote-host
https://code.visualstudio.com/docs/remote/create-dev-container#_dockerfile

https://code.visualstudio.com/remote/advancedcontainers/add-local-file-mount

## Update Git

https://oracle-base.com/articles/linux/git-2-installation-on-linux



## Command

```
docker build . -t realtimesdk_java
docker build . -t realtimesdk_java -f DockerfileJava
```

```
docker run -it --name rtsdkjava realtimesdk_java
```

```
docker pull refinitivapis/realtimesdk_java

docker run -it --name rtsdkjava refinitivapis/realtimesdk_java

docker run -it --name rtsdkjava -v C:\drive_d\Project\Code\RTSDK_Remote_Container\test:/opt/refinitiv/Real-Time-SDK/Java refinitivapis/realtimesdk_java
docker run -it --name consumer -v C:\drive_d\Project\Code\RTSDK_Remote_Container\log:/opt/refinitiv/Real-Time-SDK/Java/log refinitivapis/realtimesdk_java

docker run -it --name provider refinitivapis/realtimesdk_java
```

```
./gradlew runconsumer100 -PvmArgs="-Djava.util.logging.config.file=/opt/refinitiv/Real-Time-SDK/Java/log/logging.properties"

./gradlew runiprovider100

```

{
	"workspaceFolder": "/opt/refinitiv/Real-Time-SDK"
}