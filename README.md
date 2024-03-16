Project Description: Deploying a Static Web Page with Maven on AWS EC2 Instance Running Ubuntu

Introduction:
In modern web development, deploying static web pages efficiently is crucial for showcasing content or building simple web applications. AWS EC2 (Elastic Compute Cloud) provides a scalable and reliable infrastructure for hosting applications. This project aims to demonstrate the deployment of a static web page using Maven build automation tool on an AWS EC2 instance running Ubuntu.

Objective:
The primary objective of this project is to deploy a static web page onto an AWS EC2 instance utilizing Ubuntu as the operating system. Maven will be employed to automate the build process and manage dependencies effectively.

Technologies Used:

    AWS EC2: Provides scalable compute capacity in the cloud.
    Ubuntu: A popular Linux distribution known for its stability and versatility.
    Maven: A build automation tool used primarily for Java projects, but capable of managing dependencies for other types of projects.
    HTML/CSS/JavaScript: Basic web development technologies for creating the static web page.

Project Steps:

    Set up AWS EC2 Instance:
        Log in to the AWS Management Console.
        Launch a new EC2 instance, selecting Ubuntu as the operating system.
        Configure security groups to allow inbound traffic on port 80 (HTTP) and port 22 (SSH).
        Retrieve the public IP address of the EC2 instance.

    Connect to EC2 Instance:
        SSH into the EC2 instance using the key pair generated during instance creation.
        Update the Ubuntu package repository: sudo apt update.

    Install Maven:
        Install Maven on the EC2 instance: sudo apt install maven.
        Verify the installation: mvn -version.

    Prepare Static Web Page:
        Create a simple static web page using HTML, CSS, and JavaScript.
        Organize the project structure with necessary directories (e.g., src/main/webapp).
        Ensure all required assets (images, stylesheets, scripts) are included.

    Configure Maven Project:
        Create a Maven project or use an existing one.
        Add dependencies for any required plugins (e.g., maven-war-plugin).
        Configure the build process to include static web page files in the WAR (Web ARchive) package.

    Build and Package:
        Run Maven to compile the project and package it into a WAR file: mvn package.
        Verify that the WAR file is generated successfully.

    Access the Web Page:
        Open a web browser and navigate to the public IP address of the EC2 instance.
        The deployed static web page should be accessible.

Conclusion:
This project demonstrates the deployment of a static web page using Maven build automation on an AWS EC2 instance running Ubuntu. By following these steps, developers can efficiently deploy static content to the cloud, leveraging the scalability and reliability offered by AWS infrastructure.
