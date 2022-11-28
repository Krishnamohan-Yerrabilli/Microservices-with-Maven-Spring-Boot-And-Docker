# Microservices-with-Maven-Spring_Boot-And-Docker
In this repo we will learn how to use Spring Boot to create a microservice that connects to a PostgreSQL database running on Docker.

### Open your terminal its easy to provision our packages and libraries (here your seeing an vm, for further intellij installation purpose)
you need to do all your work in your local machine so upcoming installations will be install in lm

![2 maven ](https://user-images.githubusercontent.com/58173938/204171631-404a2b93-9f75-400b-a2fe-2980aa7e7e6f.png)

### To install maven go through this [file](https://github.com/Krishnamohan-Yerrabilli/Microservices-with-Maven-Spring_Boot-And-Docker/blob/main/Setup/commands.txt) 

![3 maven installation commands](https://user-images.githubusercontent.com/58173938/204171809-bb651a87-a707-4bb3-8ecc-1a66587824fc.png)

### Create a new directory for the project and execute below Maven goal

You may change the groupid, artifactid, version if you want.

```
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



