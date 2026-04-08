# Crypto Data Pipeline & Analytics Dashboard

## Overview
This project is an end-to-end ETL pipeline for cryptocurrency data. It collects real-time data, processes it, and shows insights through a dashboard. The project demonstrates basic data engineering concepts like data ingestion, processing, and visualization.

## Architecture
- Data Ingestion: Collects real-time crypto data  
- Streaming: Processes and moves data  
- Processing: Cleans and analyzes data  
- Storage: Saves data in database  
- Orchestration: Manages workflows using Airflow  
- Visualization: Displays data in dashboard  

## Tech Stack
- Apache Airflow  
- Apache Kafka & Zookeeper  
- Apache Spark  
- MinIO  
- PostgreSQL  
- Python (FastAPI)  
- React  
- Docker & Docker Compose  

## Project Structure
- airflow/ → Airflow setup  
- dags/ → Workflow scripts  
- spark-jobs/ → Processing jobs  
- dashboard/ → Backend & frontend  
- postgres/ → Database setup  

## Setup & Installation

### Prerequisites
- Docker  
- Docker Compose  

### Steps
1. Clone repository:
git clone <your-repo-link>  
cd <project-folder>  

2. Create .env file:
POSTGRES_USER=airflow  
POSTGRES_PASSWORD=airflow  
POSTGRES_DB=airflow  
AIRFLOW_DB_USER=airflow  
AIRFLOW_DB_PASSWORD=airflow  
AIRFLOW_DB_NAME=airflow  
AIRFLOW_ADMIN_USER=admin  
AIRFLOW_ADMIN_PASSWORD=admin  
AIRFLOW_ADMIN_EMAIL=admin@example.com  
MINIO_ROOT_USER=minio  
MINIO_ROOT_PASSWORD=minio123  
API_KEY=your_api_key  

3. Run project:
docker compose up --build  

## Access Services
- Airflow: http://localhost:8080  
- Spark: http://localhost:8090  
- MinIO: http://localhost:9011  
- Dashboard: http://localhost:3000  

## Key Features
- Real-time data pipeline  
- Distributed processing  
- Workflow automation  
- Scalable Docker setup  
- Interactive dashboard  

## Use Cases
- Crypto price tracking  
- Real-time analytics  
- Data engineering learning  

## Future Improvements
- Add alerts  
- More data sources  
- Better dashboard  
- Cloud deployment  

## Author
Veena Akkenapalli
