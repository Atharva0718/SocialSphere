SocialSphere – A Facebook-like Social Media Web App

SocialSphere is a lightweight social media platform built using Java EE (Servlets + JSP) with Maven, JDBC, H2 Database, and Tomcat.
It allows users to create accounts, post updates, view others’ posts, manage profiles, and interact inside a simple, clean UI.

🚀 Features

User Registration & Login

Create, Edit & Delete Posts

View Feed of All User Posts

Like / Comment System (optional based on your implementation)

User Profile Page

Session Management

Database-backed storage using H2 DB

Fully deployable WAR file on Apache Tomcat

Clean MVC Structure with Servlets + JSP

🛠️ Tech Stack
Backend

Java 8+

Java EE Servlets

JSP

JDBC

Maven (Project Build Tool)

Frontend

HTML

CSS

JSP Pages

Database

H2 Database (Lightweight, file-based DB)

Server

Apache Tomcat 9/10

IDE

IntelliJ IDEA Community Edition

📂 Project Structure
SocialSphere/
 ├── src/main/java/
 │    └── com.socialsphere.*   # Servlets & Logic
 ├── src/main/webapp/
 │    ├── views/                # JSP pages
 │    ├── assets/               # CSS, images
 │    └── WEB-INF/              # web.xml
 ├── pom.xml
 └── README.md

⚙️ How to Run the Project (Step-by-Step)
1. Clone the repository
git clone https://github.com/your-username/SocialSphere.git
cd SocialSphere

2. Open in IntelliJ IDEA

Go to:
File → Open → Select Project Folder

IntelliJ will automatically load Maven dependencies.

3. Build the Project

In IntelliJ:

Maven → Lifecycle → package

This will generate the file:

target/SocialSphere.war

4. Deploy Manually on Tomcat

Go to your Tomcat installation folder

Open the webapps/ directory

Copy the WAR file:

SocialSphere.war → apache-tomcat/webapps/


Start Tomcat using:

bin/startup.bat   (Windows)
bin/startup.sh    (Linux/Mac)


Open in browser:

http://localhost:8080/SocialSphere

🛢️ Database – H2 Setup

The H2 configuration is handled automatically inside the code.
You can access the H2 console using:

http://localhost:8080/SocialSphere/h2-console


Use the database settings defined in the project (jdbc:h2:~/socialsphere or in-memory based on your config).

📸 Screenshots

(Add screenshots if available)

/screenshots
 ├── login.png
 ├── feed.png
 ├── profile.png

📘 What I Learned

Building Java EE applications using Servlets & JSP

Managing backend logic with MVC pattern

Integrating H2 database using JDBC

Packaging and deploying WAR files

Session handling and authentication flows

Hosting a complete web app on Tomcat
