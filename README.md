<h1 align="center">Leveraging-Elastic-Beanstalk-and-Configuring-and-Hosting-Full-Stack-Application
</h1>
<p align="center">
  <a href="http://temp-url.com" target="_blank">
    <img alt="Documentation" src="https://img.shields.io/badge/documentation-yes-brightgreen.svg" />
  </a>
</p>

This repository contains a Laravel web application hosted on AWS, designed to showcase the integration of various AWS services including EC2, RDS, and Elastic Beanstalk.

## Project Overview
The project consists of a web application that demonstrates how to set up a Laravel framework in an AWS environment, leveraging EC2 for hosting and RDS for database management.  

## Features
- **Laravel Framework**: Built on the popular Laravel framework for robust web applications.
- **AWS Integration**: Utilizes EC2 for hosting, RDS for database management, and Elastic Beanstalk for deployment.
- **Modular Structure**: The application is structured for easy understanding and maintenance.
- **Error Handling & Logging**: Includes error handling and logging features for reliability.
  
## Table of Contents
- [Architecture](#architecture)
- [Code Layout](#code-layout)
- [Dependencies](#dependencies)
- [Setup Steps](#setup-steps)
- [Configuration Options](#configuration-options)
- [Deployment](#deployment)
- [Change Process](#change-process)
- [Contact](#contact)
  
## Architecture

![Architecture Diagram](path/to/architecture-diagram.png) <!-- Replace with actual image path -->  

## Code Layout

```plaintext
Project2-1stop 
├── .env # Environment configuration file. 
├── app # Application source code. 
├── bootstrap # Bootstrap the application. 
├── config # Application configuration files. 
├── database # Database migrations and seeders. 
├── public # Publicly accessible files, including index.php. 
├── resources # Views and assets. 
├── routes # Application routes. 
├── storage # Application storage for logs and files. 
├── tests # Automated tests for the application. 
├── vendor # Composer dependencies. 
└── README.md # Project documentation.

1 directory, 13 files
```
## Dependencies
- **PHP**: Version 8.1 or higher.
- **Composer**: Dependency manager for PHP to launch Laravel webpage.
- **Laravel**: Version 8 or higher.
- **AWS SDK for PHP**: For AWS integrations.

## Setup Steps
1. **Web Application Setup**
   - Download and install PHP and Composer.
   - Create a new Laravel project using Composer.
2. **GitHub Setup**
   - Create a GitHub repository and push the Laravel project files.
3. **EC2 Instance Creation**
   - Launch an EC2 instance with Amazon Linux 2.
4. **Installation on EC2**
   - Install PHP, Git, Composer, and Apache on the EC2 instance.
5. **RDS Database Setup**
   - Create an RDS instance using MariaDB.
6. **Elastic Beanstalk Setup**
   - Deploy the application using AWS Elastic Beanstalk.

## Configuration Options
The `.env` file includes the following configuration options:

```plaintext
DB_CONNECTION=mariadb
DB_HOST=<RDS_ENDPOINT>
DB_PORT=3306
DB_DATABASE=<DATABASE_NAME>
DB_USERNAME=<DB_USERNAME>
DB_PASSWORD=<DB_PASSWORD>
```
After creation of RDS, we will get the username, password, DB name, db endpoint which we need to put in .env file.  

**Reason:** The RDS database is meant to store and manage the application's persistent data. In Laravel, the database is used to manage things like user data, settings, and other resources through database migrations and models. Typically, Laravel applications use databases like MySQL or MariaDB, and in this case, the RDS MariaDB instance would serve as the central database for the application to store all the data.

## Deployment
To deploy the application on Elastic Beanstalk:
1. Create an IAM user and attach necessary policies.
2. Package the Laravel application and upload it to Elastic Beanstalk.
3. Configure the environment settings and launch the application.

## Change Process
Follow these steps for making changes to the project:
1. Create a feature branch for your changes.
2. Make necessary changes and commit them.
3. Push your branch to the remote repository.
4. Create a pull request for review.
5. Once approved, merge the changes into the main branch.

## Contact
👤 **Rupam Patwari**  
Email: [patwarirupam@gmail.com](mailto:patwarirupam@gmail.com)


