# ☁️ Cloud File Storage System

## Live Demo

**Deployed Application:**
https://cloud-file-storage-system-secw.onrender.com

---

## Project Overview

Cloud File Storage System is a cloud-based web application that allows users to securely upload, store, manage, and share files using Amazon S3. The application uses Google OAuth 2.0 for user authentication and is deployed on Render for public access.

The project demonstrates the integration of cloud storage services, authentication mechanisms, and web application deployment in a real-world environment.

---

## Problem Statement

Managing files securely and accessing them from anywhere is a common requirement for individuals and organizations. Traditional local storage systems limit accessibility and sharing capabilities.

This project provides a simple cloud-based solution where authenticated users can upload files to cloud storage, access them online, share them through secure links, and manage them efficiently.

---

## Objectives

* Build a cloud-based file storage application.
* Implement secure user authentication.
* Store files using AWS S3.
* Allow users to upload, download, delete, and share files.
* Deploy the application on a cloud platform.

---

## Features

### Authentication

* Google OAuth 2.0 Login
* Secure user authentication
* User session management
* Logout functionality

### File Management

* Upload files to AWS S3
* View uploaded files
* Download files
* Delete files
* Generate secure shareable links

### Cloud Features

* AWS S3 cloud storage integration
* S3 bucket versioning enabled
* Secure access using IAM credentials

### Deployment

* Hosted on Render
* Accessible through a public URL

---

## Technology Stack

### Frontend

* HTML5
* CSS3

### Backend

* Python
* Flask

### Cloud Services

* Amazon S3
* Google OAuth 2.0
* Render

### Libraries Used

* Flask
* Boto3
* Authlib
* Gunicorn

---

## System Architecture

User
↓
Google OAuth Authentication
↓
Flask Application
↓
AWS S3 Storage
↓
File Management Operations

---

## Project Workflow

### User Authentication

1. User opens the application.
2. User clicks "Login with Google".
3. Google verifies the user's identity.
4. User is redirected to the dashboard.

### File Upload

1. User selects a file.
2. Flask receives the file.
3. File is uploaded to AWS S3.
4. File appears in the dashboard.

### File Download

1. User clicks Download.
2. Flask generates a temporary S3 download URL.
3. File is downloaded securely.

### File Sharing

1. User clicks Share.
2. Flask creates a pre-signed URL.
3. User can share the generated link.

### File Deletion

1. User clicks Delete.
2. File is removed from the S3 bucket.
3. Dashboard updates automatically.

---

## Project Structure

CloudFileStorage

├── app.py

├── requirements.txt

├── Procfile

├── .gitignore

├── templates

│   ├── login.html

│   └── index.html

└── README.md

---

## AWS Services Used

### Amazon S3

Purpose:

* Cloud file storage
* File retrieval
* File sharing
* File versioning

### IAM

Purpose:

* Secure access control
* Programmatic access through Access Keys

---

## Google OAuth 2.0

Used for:

* User authentication
* Secure login
* User identity verification

Benefits:

* No password storage required
* Secure and reliable authentication
* Industry-standard login mechanism

---

## Deployment

The application is deployed using Render.

### Deployment Steps

1. Push source code to GitHub.
2. Connect GitHub repository to Render.
3. Configure environment variables.
4. Deploy Flask application using Gunicorn.
5. Configure Google OAuth redirect URLs.

---

## Environment Variables

```env
AWS_ACCESS_KEY=YOUR_AWS_ACCESS_KEY
AWS_SECRET_KEY=YOUR_AWS_SECRET_KEY

BUCKET_NAME=YOUR_BUCKET_NAME
REGION=ap-south-1

GOOGLE_CLIENT_ID=YOUR_CLIENT_ID
GOOGLE_CLIENT_SECRET=YOUR_CLIENT_SECRET

SECRET_KEY=YOUR_SECRET_KEY
```

---

## Installation and Setup

### Clone Repository

```bash
git clone <repository-url>
cd CloudFileStorage
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Application

```bash
python app.py
```

### Open Browser

```text
http://127.0.0.1:5000
```

---

## Learning Outcomes

Through this project, the following concepts were learned:

* Cloud Computing Fundamentals
* AWS S3 Integration
* IAM Access Management
* OAuth Authentication
* Flask Web Development
* Cloud Deployment
* Environment Variables
* Secure File Handling

---

## Future Enhancements

* User-specific file folders
* File search functionality
* File preview support
* Storage usage analytics
* Multi-file upload
* Database integration
* Role-based access control
* Email notifications

---

## Conclusion

The Cloud File Storage System successfully demonstrates the integration of modern cloud technologies with web application development. The project provides secure authentication, cloud-based file management, and public deployment while maintaining simplicity and scalability.

This project serves as a practical implementation of cloud computing concepts and real-world application deployment.
