# Provision

To build the Microservice first we need to have a VM, select `ubuntu 16.04` on top of that we install our dependencies which we need

### Create a Maven Project in the Virtual Machine which is running on GCP, you can use any Cloud_Provider

![1 maven project](https://user-images.githubusercontent.com/58173938/204171534-14b19ffe-a34f-4225-9a9c-74cc26580ef4.png)

### SSH into VM though its easy to provision our packages and libraries 

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

## ❤ Show your support

Give a ⭐️ if this project helped you, Happy learning!
