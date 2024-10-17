<h1 align="center">Leveraging AWS: Hosting a Full-Stack Laravel Application on Elastic Beanstalk</h1>

<p align="center">
  <a href="http://temp-url.com" target="_blank">
    <img alt="Documentation" src="https://img.shields.io/badge/documentation-yes-brightgreen.svg" />
  </a>
  <a href="http://temp-url.com/deploy" target="_blank">
    <img alt="AWS Deployment" src="https://img.shields.io/badge/deployed%20on-AWS-blue" />
  </a>
</p>

<p align="center">
  <strong>Build, Deploy, and Scale Laravel Applications Seamlessly on AWS</strong>  
</p>

This repository contains a **full-stack Laravel web application** hosted on **AWS**, showcasing a modern and scalable architecture using **EC2**, **RDS**, and **Elastic Beanstalk**. The project demonstrates how to configure, deploy, and manage a Laravel application in a cloud-native environment.

---

## 🚀 **Project Overview**

This project aims to provide a **step-by-step guide** to building and deploying a **Laravel web application** in AWS. It integrates **AWS services** like EC2 for hosting, RDS for database management, and Elastic Beanstalk for automated scaling and easy deployment.  

---

## 🌟 Key Features

- **🛠 Laravel 8.x**: Utilizing the latest features of this powerful PHP framework
- **☁️ AWS Integration**: 
  - **EC2** for flexible compute capacity
  - **RDS (MariaDB)** for managed relational database
  - **Elastic Beanstalk** for automated deployment and scaling
- **🔐 Security-First Approach**: Implements AWS IAM policies and best security practices
- **📘 Comprehensive Documentation**: Detailed setup and deployment instructions

---

## 🏃‍♂️ **Quick Start**

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/your-repo.git
   ```
2. Install dependencies:
   ```bash
   composer install
   ```
3. Configure your `.env` file with AWS credentials and database information
4. Run migrations:
   ```bash
   php artisan migrate
   ```
5. Deploy to Elastic Beanstalk (see [Deployment](#deployment-process) section)
   
---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Architecture](#architecture)
4. [Code Layout](#code-layout)
5. [Dependencies](#dependencies)
6. [Setup Steps](#setup-steps)
7. [Configuration Options](#configuration-options)
8. [Deployment](#deployment)
9. [Change Process](#change-process)
10. [Contact](#contact)

---
## 🏗 **Architecture**

![image](https://github.com/user-attachments/assets/f4b67070-16df-42e1-bdf0-34f7450ff80d)  

The application is hosted on AWS EC2, connected to a MariaDB RDS instance, and is packaged and deployed using Elastic Beanstalk for automatic scaling and deployment.  

---

## 🗂 **Code Layout**

```plaintext
Project
├── project-Laravel        # contains all the files of Laravel webpage to deploy.
├── doc.pdf                # documentation of detailed steps followed with relevant screenshots.
└── README.md              # Project overview.
```
---

## 📦 **Dependencies**
- **PHP**: Version 8.1 or higher.
- **Composer**: PHP dependency manager.
- **Laravel**: Version 8 or higher.
- **AWS SDK for PHP**: To integrate with AWS services like RDS and S3.

---

## ⚙️ **Setup Steps**
1. **Web Application Setup**  
   - Install PHP and Composer locally.
   - Create a Laravel project using Composer.
  
2. **GitHub Repository**  
   - Create a repository and push your Laravel project files.

3. **EC2 Instance Setup**  
   - Launch an EC2 instance with **Amazon Linux 2**.
   - Install PHP, Composer, Apache, and Git.

4. **Database Configuration (RDS)**  
   - Create an RDS instance using **MariaDB** for database management.
   
5. **Elastic Beanstalk Deployment**  
   - Use AWS Elastic Beanstalk to package and deploy the Laravel application.

---

## 🔧 **Configuration Options**

The `.env` file should include your RDS connection information:

```plaintext
DB_CONNECTION=mariadb
DB_HOST=<RDS_ENDPOINT>
DB_PORT=3306
DB_DATABASE=<DATABASE_NAME>
DB_USERNAME=<DB_USERNAME>
DB_PASSWORD=<DB_PASSWORD>
```
Ensure to retrieve the database credentials and endpoint after creating RDS instance and insert them into the .env file for Laravel.

**Reason:** The RDS database is meant to store and manage the application's persistent data. In Laravel, the database is used to manage things like user data, settings, and other resources through database migrations and models. Typically, Laravel applications use databases like MySQL or MariaDB, and in this case, the RDS MariaDB instance would serve as the central database for the application to store all the data.

---

## 🚀 **Deployment Process**

1. **IAM User Setup**  
   - Create an IAM user with permissions for **Elastic Beanstalk**, **EC2**, and **RDS**.
  
2. **Elastic Beanstalk Deployment**  
   - Upload the Laravel application package to **Elastic Beanstalk**.
   - Set up environment variables, security groups, and scaling policies.

---

## 🔄 **Change Management Process**
1. **Create a New Feature Branch**: Use a feature-based branching model to isolate changes.
2. **Commit and Push Changes**: Push changes to GitHub.
3. **Pull Request and Review**: Open a pull request for peer review.
4. **Merge to Main Branch**: Once approved, merge the changes into the `main` branch.

---

## 🆘 Troubleshooting & FAQ

**Q: How do I resolve "Connection refused" errors with RDS?**  
**A:** Ensure that your security group settings allow inbound traffic on the database port (typically 3306 for MySQL/MariaDB) from your EC2 instance's security group.

---


## 💼 **Contact**

If you are interested in discussing this project further or exploring more about my technical skills, feel free to reach out!

👤 **Rupam Patwari**  
📧 [patwarirupam@gmail.com](mailto:patwarirupam@gmail.com)  
📍 LinkedIn: [My LinkedIn Profile](https://www.linkedin.com/in/rupam-patwari-431b53206/)

---



