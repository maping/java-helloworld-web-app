# A Java Hello World Web Application
[![Build Status](https://dev.azure.com/maping930883/java-helloworld-web-app/_apis/build/status/java-helloworld-web-app-Maven-CI?branchName=master)](https://dev.azure.com/maping930883/java-helloworld-web-app/_build/latest?definitionId=26&branchName=master)

## 1. Create a repo manually

### 1.1 Create a repo on GitHub
Click "Repositories",then click "New" button,input "java-helloworld-web-app", leave all other input as default, click "Create repository".

### 1.2 Create a Java helloword web app by Maven
```console
$ cd /mnt/c/Users/pinm/code/maven/
$ mvn archetype:generate -DgroupId=com.mwit.javawebapp -DartifactId=java-helloworld-web-app -DarchetypeArtifactId=maven-archetype-webapp -Dversion=1.0-SNAPSHOT -DinteractiveMode=false
```

### 1.3 Init repo 
```console
$ cd /mnt/c/Users/pinm/code/maven/java-helloworld-web-app
$ code README.md
$ git init
$ git add -A
$ git commit -m "add java maven archetype web app"
$ git remote add origin https://github.com/maping/java-helloworld-web-app.git 
$ git push -u origin master
```

## 2. Create a repo automaticly by GitHub CLI

### 2.1 Download and install GitHub CLI
https://cli.github.com/

### 2.2 Generate a Personal Access Token with repo operation privilege
https://github.com/settings/tokens

### 2.3 Create a Java helloworld web app by Maven
```console
$ cd /mnt/c/Users/pinm/code/maven/
$ mvn archetype:generate -DgroupId=com.mwit.javawebapp -DartifactId=java-helloworld-web-app -DarchetypeArtifactId=maven-archetype-webapp -Dversion=1.0-SNAPSHOT -DinteractiveMode=false
```

### 2.4 Create a repo
```console
$ cd /mnt/c/Users/pinm/code/github/
$ gh repo create java-helloworld-web-app --public --confirm
```

### 2.5 Copy files
```console
$ cp -r /mnt/c/Users/pinm/code/maven/java-helloworld-web-app/* /mnt/c/Users/pinm/code/github/java-helloworld-web-app
$ cd /mnt/c/Users/pinm/code/github/java-helloworld-web-app
$ code README.md
$ git add -A
$ git commit -m "add java maven archetype web app"
$ git push -u origin master
```

## 3. Create a Maven CI pipeline

## 4. Create a Maven CI&CD pipeline

## 5. Create a Self-Hosted VM CI pipeline

## 6. Create a Self-Hosted Docker CI pipeline
### 6.1 Run as a standalone Docker container
### 6.2 Deploy and run on Kubernetes

## 7. Delete repo
Click repo "maping/java-helloworld-web-app", then click "Settings", then drop down to "Danger Zone", click "Delete this repository".
