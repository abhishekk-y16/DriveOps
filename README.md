# 🚗 DriveFlow – Car Rental Application with AWS Deployment Pipeline

## Project Overview

DriveFlow is a cloud-based car rental application designed with a production-style deployment workflow on AWS. The project focuses not only on the application's functionality but also on implementing secure infrastructure, automated deployment practices, and scalable cloud architecture.

## AWS Implementation

### Amazon S3

The application source code and deployment assets are stored in an Amazon S3 bucket. EC2 instances retrieve only the required application files during deployment, providing a centralized and reliable storage solution.

### IAM Roles

Instead of using access keys, EC2 instances are assigned IAM Roles with carefully scoped permissions. Each instance receives only the minimum level of access necessary to interact with AWS services, following the Principle of Least Privilege.

### Amazon Machine Image (AMI)

A custom Amazon Machine Image (AMI) is created after configuring the application environment. This allows new EC2 instances to launch with the application stack already installed and configured, reducing deployment time and ensuring consistency across instances.

### Amazon SNS

Amazon Simple Notification Service (SNS) is configured to send deployment and infrastructure notifications. Whenever deployment-related events or scaling activities occur, subscribers receive automated alerts, making it easier to monitor application operations.

## Key Features

* Secure application deployment using AWS IAM Roles
* Centralized application storage with Amazon S3
* Custom AMIs for faster and consistent server provisioning
* Automated notifications using Amazon SNS
* Scalable and production-oriented AWS architecture
* Infrastructure designed following AWS security best practices

## Technologies Used

* AWS EC2
* Amazon S3
* AWS IAM
* Amazon Machine Image (AMI)
* Amazon SNS
* Linux
* Git & GitHub

## Learning Outcomes

This project strengthened my understanding of:

* Secure authentication between AWS services using IAM Roles
* Managing deployment assets with Amazon S3
* Creating reusable machine images for rapid infrastructure provisioning.
* Configuring cloud-based notification services with SNS.
* Building and deploying applications using AWS production best practices.
