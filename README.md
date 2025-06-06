<project xmlns="http://maven.apache.org/POM/4.0.0"
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-
4.0.0.xsd">
<modelVersion>4.0.0</modelVersion>
 <groupId>com.example</groupId>
 <artifactId>simple-project</artifactId>
<version>1.0-SNAPSHOT</version>
<dependencies>
<!-- Add your dependencies here -->
</dependencies>
</project>
<dependencies>
<dependency>
<groupId>org.seleniumhq.selenium</groupId>
<artifactId>selenium-java</artifactId>
<version>3.141.59</version>
</dependency>
<dependency>
<groupId>org.testng</groupId>
<artifactId>testng</artifactId>
<version>7.4.0</version>
<scope>test</scope>
</dependency>
</dependencies>

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>My Simple Website</title>
<link rel="stylesheet" href="style.css">
</head>
 <body>
<header>
<img src="logo.png" alt="Logo">
</header>
<h1>Welcome to My Simple Website</h1>
</body>
</html>

body {
font-family: Arial, sans-serif;
background-color: #f4f4f4;
DevOps Lab Manual
text-align: center;
 }
header img {
width: 100px;
}

git init
git add .
git commit -m "Initial commit"
git remote add origin <your-repository-url>
git push -u origin master

<build>
<plugins>
<plugin>
<groupId>org.apache.maven.plugins</groupId>
<artifactId>maven-resources-plugin</artifactId>
<version>3.2.0</version>
 <executions>
<execution>
<phase>prepare-package</phase> <!-- Before packaging -->
<goals>
<goal>copy-resources</goal>
</goals>
<configuration>
<outputDirectory>${project.basedir}/docs</outputDirectory> <!-- Deploy to /docs
<resources>
<resource>
<directory>src/main/resources</directory>
<includes>
<include>**/*</include> <!-- Copy all files in src/main/resources -->
</includes>
</resource>
</resources>
</configuration>
</execution>
</executions>
</plugin>
</plugins>
</build>

mvn clean install
git add docs/*
git commit -m "Deploy site to GitHub Pages"
git push origin master
https://<your-github-username>.github.io/<your-repository-name>/
