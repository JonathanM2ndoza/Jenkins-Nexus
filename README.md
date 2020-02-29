# Jenkins Integration with Nexus

## Prerequisites
* Java version 1.8.0_221
* Git version 2.23.0
* Apache Maven 3.6.0
* Jenkins version 2.176.3
* Nexus version 2.14.16-01

### 1.- Create Jenkins Freestyle Project 

![Screenshot](prtsc/Jenkins-Nexus-1.png)

Specify GIT repository

![Screenshot](prtsc/Jenkins-Nexus-1.1.png)

Set up Maven tasks

![Screenshot](prtsc/Jenkins-Nexus-1.2.png)

Build Project

![Screenshot](prtsc/Jenkins-Nexus-1.3.png)

pom.xml file

![Screenshot](prtsc/Jenkins-Nexus-1.4.png)

### 2.- Create Nexus Repository 

![Screenshot](prtsc/Jenkins-Nexus-2.png)

Hosted (Maven2)

![Screenshot](prtsc/Jenkins-Nexus-2.1.png)

Create Repository Snapshot

![Screenshot](prtsc/Jenkins-Nexus-2.2.png)

Create Repository Release

![Screenshot](prtsc/Jenkins-Nexus-2.3.png)

![Screenshot](prtsc/Jenkins-Nexus-2.4.png)

### 3.- Update pom.xml file with Repository Snapshot and Repository Release

![Screenshot](prtsc/Jenkins-Nexus-3.png)

### 4.- Update settings.xml file in /var/lib/jenkins/.m2/ with nexus credentials

![Screenshot](prtsc/Jenkins-Nexus-4.png)

### 5.- Add task deploy Maven in Jenkins (Goals)

![Screenshot](prtsc/Jenkins-Nexus-5.png)

Build Project in Jenkins

![Screenshot](prtsc/Jenkins-Nexus-5.1.png)

See the file api-customer-2.0-SNAPSHOT.jar in Nexus
![Screenshot](prtsc/Jenkins-Nexus-5.2.png)






















