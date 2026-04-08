Crypto Data Pipeline & Analytics Dashboard
Overview
This project is an end-to-end real-time data engineering pipeline designed to ingest, process, and visualize cryptocurrency market data. It demonstrates modern data engineering practices including streaming, distributed processing, workflow orchestration, and dashboarding.

The system is built to handle real-time data flow, transform it into analytical insights, and present it through an interactive dashboard.
Architecture
The pipeline follows a modular and scalable architecture:
Data Ingestion
Real-time cryptocurrency data is collected using scheduled workflows and published to a streaming platform.
Streaming Layer
Streaming jobs consume incoming data and store it in a data lake in optimized formats.
Processing and Analytics
Batch and streaming transformations are applied to compute trends, price movements, and insights.
Storage Layer
Processed data and metadata are stored in a relational database for efficient querying.
Orchestration
Workflow scheduling, monitoring, and dependency management are handled through a workflow orchestrator.
Visualization
A dashboard provides real-time insights and analytics through a user-friendly interface.

**Tech Stack**
Orchestration: Apache Airflow
Streaming and Messaging: Apache Kafka, Zookeeper
Processing Engine: Apache Spark
Data Lake: MinIO (S3-compatible)
Database: PostgreSQL
Backend API: Python (FastAPI)
Frontend: React
Containerization: Docker, Docker Compose

**Project Structure**
airflow/ → Airflow setup and configuration
dags/ → Workflow definitions for data ingestion
spark-jobs/ → Streaming and batch processing scripts
dashboard/ → Backend API and frontend UI
postgres/ → Database initialization scripts

Setup and Installation
Prerequisites
Docker
Docker Compose
1. Clone the Repository
git clone <your-repo-link>
cd <project-folder>
2. Configure Environment Variables
**Create a .env file in the root directory:**
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
**3. Run the Application**
docker compose up --build
Access Services
Airflow UI: http://localhost:8080
Spark Master: http://localhost:8090
MinIO Console: http://localhost:9011
Dashboard: http://localhost:3000
**Key Features**
Real-time data ingestion and streaming pipeline
Distributed processing using Spark cluster
Workflow orchestration with Airflow
Scalable architecture using Docker containers
Data persistence using volumes
Interactive dashboard for analytics
**Use Cases**
Cryptocurrency price tracking
Real-time analytics pipelines
Data engineering learning project
Streaming architecture demonstrations
**Future Enhancements**
Add alerting system for price spikes
Integrate additional data sources
Improve dashboard visualizations
Deploy to cloud (AWS, GCP, or Azure)
