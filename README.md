# 🚀 Multi-Tier Java Web Application Project

This project demonstrates a **multi-tier Java web application architecture** with integrated DevOps practices including build automation, configuration management, and local infrastructure provisioning.

---

## 📌 Project Overview

This is a **3-tier web application** consisting of:

* **Web Layer** → Nginx (Reverse Proxy)
* **Application Layer** → Apache Tomcat (Spring MVC Application)
* **Data Layer** → MySQL Database

Additional components:

* **Memcached** → Caching
* **RabbitMQ** → Messaging Queue
* **Elasticsearch** → Search functionality

---

## 🧰 Prerequisites

Ensure the following are installed:

* JDK 17 / 21
* Maven 3.9
* MySQL 8

---

## 🛠️ Technologies Used

* Spring MVC
* Spring Security
* Spring Data JPA
* JSP (Frontend)
* Apache Tomcat
* MySQL
* Memcached
* RabbitMQ
* Elasticsearch
* Maven (Build Tool)

---

## 🗄️ Database Setup

This project uses **MySQL** as the backend database.

### 📥 Import Database

SQL dump file location:

```bash
src/main/resources/db_backup.sql
```

### ▶️ Import Command:

```bash
mysql -u <username> -p accounts < db_backup.sql
```

---

## ⚙️ Build Application

To build the project and generate WAR file:

```bash
mvn clean install
```

Output:

```bash
target/*.war
```

---

## 🚀 Deployment Options

### 🔹 1. Local Setup using Vagrant

This project supports local infrastructure simulation using Vagrant.

To start:

```bash
vagrant up
```

---

### 🔹 2. Deployment using Apache Tomcat

* Copy WAR file to Tomcat webapps directory
* Start Tomcat server

---

### 🔹 3. CI/CD Pipeline

This project includes a pipeline configuration for Jenkins.

Pipeline stages:

* Build
* Test
* Deploy

---

## 🔄 Application Flow

User → Web Server → Application Server → Database

With integrations:

* Cache (Memcached)
* Messaging (RabbitMQ)

---

## 📁 Project Structure

* `src/` → Application source code
* `pom.xml` → Maven configuration
* `Jenkinsfile` → CI/CD pipeline
* `ansible/` → Automation scripts
* `vagrant/` → Local infrastructure setup

---

## 💡 Key Highlights

* Multi-tier architecture implementation
* DevOps integration with CI/CD
* Infrastructure automation using Ansible
* Local environment simulation using Vagrant

---

## 📌 Future Enhancements

* AWS deployment using EC2, RDS, and ALB
* Infrastructure as Code using Terraform
* Docker containerization
* Monitoring with Prometheus & Grafana

---

## 👨‍💻 Author

This project was implemented and enhanced as part of hands-on DevOps and Cloud learning.

---
