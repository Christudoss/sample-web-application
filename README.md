Jenkinsfile5 allows you to use Dockerfile to build maven docker container for build purpose. The others are original from Deekshit that builds from docker container from docker registry.

This is a sample Web Application to use during Continuous Integration demos.

# Build Instruction

```
mvn3 clean package
```

# Deploy instruction

Deploy ```target/WebApp.war``` on Tomcat
 
