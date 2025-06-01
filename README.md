# earthquake
Проект по созданию ETL-пайплайна с использованием современных инструментов Data Engineering.
## Технологический стек
- **Orchestration**: Apache Airflow
- **Data Warehouse**: PostgreSQL
- **Object Storage**: MinIO (S3-совместимое хранилище)
- **BI Visualization**: Metabase
- **Containerization**: Docker
- **Version Control**: Git

## Инфраструктура
```mermaid
graph TD
    A[Airflow] -->|Extract| B(MinIO)
    A -->|Transform| C(PostgreSQL)
    C -->|Load| D[Metabase]
