# java-tomcat-maven-example

This is an example ready-to-deploy java web application built for Tomcat using Maven and webapp-runner.

**#Install Java-11 on your machine**
yum install java-11*

**Switch to java version-11 if any other version already exists**
update-alternatives --config java
[root@ip-172-31-82-113 java-tomcat-maven-example]# update-alternatives --config java

There are 3 programs which provide 'java'.

  Selection    Command
-----------------------------------------------
*  1           /usr/lib/jvm/java-17-amazon-corretto.x86_64/bin/java
 + 2           /usr/lib/jvm/java-1.8.0-amazon-corretto.x86_64/jre/bin/java
   3           /usr/lib/jvm/java-11-amazon-corretto.x86_64/bin/java

Enter to keep the current selection[+], or type selection number: 3
[root@ip-172-31-82-113 java-tomcat-maven-example]# update-alternatives --config java

There are 3 programs which provide 'java'.

  Selection    Command
-----------------------------------------------
*  1           /usr/lib/jvm/java-17-amazon-corretto.x86_64/bin/java
   2           /usr/lib/jvm/java-1.8.0-amazon-corretto.x86_64/jre/bin/java
 + 3           /usr/lib/jvm/java-11-amazon-corretto.x86_64/bin/java


## Running Locally

(need maven and java installed)

```
mvn package
java -jar target/dependency/webapp-runner.jar target/*.war
```

The application will be available on `http://localhost:8080`.
