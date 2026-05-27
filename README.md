````markdown
# Vehicle Insurance Prediction | End-to-End MLOps Project

## Overview

This project is a production-grade End-to-End MLOps pipeline for Vehicle Insurance Prediction built using modern Machine Learning Engineering and Cloud Deployment practices.

The system automates the complete ML lifecycle including:

- Data Ingestion
- Data Validation
- Data Transformation
- Model Training
- Model Evaluation
- Model Registry
- Prediction Pipeline
- CI/CD Automation
- Docker Containerization
- Cloud Deployment on AWS

The application is deployed using FastAPI, Docker, GitHub Actions, AWS ECR, and AWS EC2 with automated CI/CD pipelines.

---

# Project Architecture

```text
MongoDB Atlas
      ↓
Data Ingestion Pipeline
      ↓
Data Validation
      ↓
Data Transformation
      ↓
Model Training
      ↓
Model Evaluation
      ↓
AWS S3 Model Registry
      ↓
Prediction Pipeline
      ↓
FastAPI Application
      ↓
Docker Container
      ↓
AWS ECR
      ↓
AWS EC2 Deployment
````

---

# Tech Stack

## Programming & ML

* Python 3.10
* Scikit-Learn
* Pandas
* NumPy

## Backend Framework

* FastAPI
* Jinja2 Templates

## Database

* MongoDB Atlas

## MLOps & DevOps

* Docker
* GitHub Actions
* CI/CD Pipelines
* Self Hosted GitHub Runner

## Cloud Services

* AWS EC2
* AWS ECR
* AWS S3
* AWS IAM

## Software Engineering Practices

* Modular Code Architecture
* Custom Exception Handling
* Logging Framework
* Configuration Management
* Artifact Management
* Environment Variables
* Reusable Components

---

# Key Features

## End-to-End ML Pipeline

Implemented a complete modular ML pipeline architecture including:

* Data ingestion
* Data validation
* Feature engineering
* Model training
* Model evaluation
* Model deployment

---

## Production Grade Project Structure

The project follows scalable MLOps folder architecture:

```text
src/
│
├── components/
├── configuration/
├── constants/
├── data_access/
├── entity/
├── exception/
├── logger/
├── pipeline/
├── aws_storage/
└── utils/
```

---

## MongoDB Data Pipeline

* Connected MongoDB Atlas database
* Fetched real-time data
* Converted key-value records into DataFrames
* Automated ingestion workflow

---

## AWS S3 Model Registry

Implemented model versioning and storage using AWS S3:

* Model upload
* Model retrieval
* Production model loading
* Cloud-based model registry system

---

## CI/CD Automation

Fully automated CI/CD pipeline using GitHub Actions.

### Continuous Integration

* Code checkout
* Docker image build
* Image push to AWS ECR

### Continuous Deployment

* Pull latest Docker image
* Deploy automatically to AWS EC2
* Self-hosted GitHub runner setup

---

## Dockerized Deployment

Application containerized using Docker for:

* Reproducibility
* Scalability
* Environment consistency
* Production deployment

---

## FastAPI Prediction Service

Interactive prediction application built using FastAPI.

Features:

* REST API support
* HTML template rendering
* Real-time predictions
* Cloud deployment ready

---

# Machine Learning Workflow

## Data Ingestion

* Fetch data from MongoDB Atlas
* Export datasets for pipeline processing

## Data Validation

* Schema validation
* Missing value checks
* Data consistency verification

## Data Transformation

* Feature engineering
* Data preprocessing
* Pipeline transformations

## Model Training

* Model training pipeline
* Estimator abstraction
* Training artifacts generation

## Model Evaluation

* Performance comparison
* Threshold-based evaluation
* Best model selection

## Model Pusher

* Push trained model to AWS S3 model registry

---

# AWS Services Used

| Service | Purpose               |
| ------- | --------------------- |
| AWS EC2 | Application Hosting   |
| AWS ECR | Docker Image Registry |
| AWS S3  | Model Registry        |
| AWS IAM | Access Management     |

---

# CI/CD Workflow

```text
GitHub Push
    ↓
GitHub Actions Triggered
    ↓
Docker Image Build
    ↓
Push Image to AWS ECR
    ↓
EC2 Self Hosted Runner Pulls Latest Image
    ↓
Container Deployment
    ↓
Application Live
```

---

# Environment Variables

Create the following environment variables:

```bash
AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
AWS_DEFAULT_REGION=
MONGODB_URL=
```

---

# Installation

## Clone Repository

```bash
git clone <repository_url>
cd vehicle-insurance-prediction
```

---

## Create Virtual Environment

```bash
conda create -n vehicle python=3.10 -y
conda activate vehicle
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Run Application Locally

```bash
python app.py
```

Application will start at:

```text
http://localhost:5000
```

---

# Docker Setup

## Build Docker Image

```bash
docker build -t vehicleproj .
```

## Run Container

```bash
docker run -p 5000:5000 vehicleproj
```

---

# GitHub Actions CI/CD

The project includes automated deployment pipelines using:

```text
.github/workflows/aws.yaml
```

Pipeline stages:

* Build
* Test
* Dockerization
* ECR Push
* EC2 Deployment

---

# Logging & Exception Handling

Implemented custom:

* Logging framework
* Exception handling classes
* Error traceability
* Debugging support

---

# Future Improvements

* MLflow Integration
* Kubernetes Deployment
* Monitoring & Alerting
* Automated Retraining
* Experiment Tracking
* Terraform Infrastructure Automation

---

# Project Highlights

* End-to-End MLOps Pipeline
* Cloud Native Deployment
* Production Ready Architecture
* CI/CD Automation
* Dockerized ML Application
* AWS Integration
* Modular Engineering Design
* FastAPI Deployment
* Model Registry Implementation

---
