# Microservices-with-Maven-Spring_Boot-And-Docker
In this repo we will learn how to use Spring Boot to create a microservice that connects to a PostgreSQL database running on Docker.

### Open your terminal its easy to provision our packages and libraries (here your seeing an vm, for further intellij installation purpose)
you need to do all your work in your local machine so upcoming installations will be install in lm

![2 maven ](https://user-images.githubusercontent.com/58173938/204171631-404a2b93-9f75-400b-a2fe-2980aa7e7e6f.png)

### To install maven go through this [file](https://github.com/Krishnamohan-Yerrabilli/Microservices-with-Maven-Spring_Boot-And-Docker/blob/main/Setup/commands.sh) 

![3 maven installation commands](https://user-images.githubusercontent.com/58173938/204171809-bb651a87-a707-4bb3-8ecc-1a66587824fc.png)

### Create a new directory for the project and execute below Maven goal

You may change the groupid, artifactid, version if you want.

```s
mvn archetype:generate -DgroupId=com.mohan.practice -DartifactId=mohanservices 
-DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false

```
### After the build completed this is going to been seen 

![4 maven](https://user-images.githubusercontent.com/58173938/204174058-fc6e6594-fd9c-4545-b1f3-ac7a951af01f.png)

### As we can see now the generate build is created as same as the artifictid

> To see the tree structure, install the package `sudo apt install tree`

![5 maven](https://user-images.githubusercontent.com/58173938/204183401-709bc350-f495-4b74-bd76-d904a6f3a115.png)

### Install intellij on your local machine

I'm using ubuntu as my lm, you can install through intellij [toolbox](https://www.jetbrains.com/help/idea/installation-guide.html)

or you can use snap as your package-manager 

For this context im using intellij-community-edition

> sudo snap install intellij-idea-ultimate --classic

![maven6](https://user-images.githubusercontent.com/58173938/204202379-729d3cc7-1860-44d2-b7f9-a15f2e0c0280.png)

### Open the pom.xml file Leave the properties and erase the dependencies.

```s
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>org.example</groupId>
    <artifactId>mohanservice</artifactId>
    <version>1.0-SNAPSHOT</version>

    <dependencies>
    </dependencies>

    <properties>
        <maven.compiler.source>19</maven.compiler.source>
        <maven.compiler.target>19</maven.compiler.target>
        <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
    </properties>

</project>
```

New Properties for plugins and dependency management

```s
 <properties>
        <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
        <maven.compiler.source>19</maven.compiler.source>
        <maven.compiler.target>19</maven.compiler.target>
        <spring.boot.maven.plugin.version>2.5.7</spring.boot.maven.plugin.version>
        <spring.boot.dependencies.version>2.5.7</spring.boot.dependencies.version>
 </properties>
 
```
Let’s add a plugin for building artifacts.

> An artifact is an element that a project can either use or produce. In Maven terminology, an artifact is an output generated after a Maven project build.

```s
<build>
  <pluginManagement><!-- lock down plugins versions to avoid using Maven defaults (may be moved to parent pom) -->
    <plugins>
      <plugin>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-maven-plugin</artifactId>
        <version>${spring.boot.maven.plugin.version}</version>
      </plugin>
    </plugins>
  </pluginManagement>
</build>
```

As we can see the dependencies are added to the parent module, if you can't able to see it
Tap on maven on left side of the window and reload

![dependencies](https://user-images.githubusercontent.com/58173938/204226069-1557fa6a-341e-4551-a342-bb0e33cba1c1.png)

## ❤ Show your support

Give a ⭐️ if this project helped you, Happy learning!

