```
akasa-data-engineer/
│
├── main.py                          # Main pipeline execution script
├── requirements.txt                  # Python dependencies
├── .env.example                     # Environment variables template
├── .gitignore                       # Git ignore rules
│
├── assets/                          # Static assets and outputs
│   ├── task_DE_new_customers.csv    # Sample customer data
│   ├── task_DE_new_orders.xml       # Sample order data
│   ├── analytics_dashboards/        # Generated visualizations
│   │   ├── dashboard_20251107_073641.png
│   │   ├── revenue_20251107_073641.png
│   │   └── regional_20251107_073641.png
│   └── reports/                     # Business reports
│       ├── business_report_20251107_043727.txt
│       └── business_report_20251107_043727.json
│
├── data/                            # Processed data storage
│   ├── bronze/                      # Raw ingested data
│   │   ├── customers_bronze_20251106_230722.parquet
│   │   └── orders_bronze_20251106_230722.parquet
│   ├── silver/                      # Cleaned and enriched data
│   │   ├── customers_silver_20251106_230722.parquet
│   │   ├── orders_silver_20251106_230722.parquet
│   │   └── processing_metadata_20251106_230722.json
│   └── gold/                        # Business KPIs and metrics
│       ├── repeat_customers_20251106_230722.parquet
│       ├── monthly_trends_20251106_230722.parquet
│       ├── regional_revenue_20251106_230722.parquet
│       ├── top_customers_30d_20251106_230722.parquet
│       └── gold_metadata_20251106_230722.json
│
├── logs/                            # Application logs
│   └── akasaair_processing.log      # Main processing log file
│
├── src/                             # Source code
│   ├── __init__.py
│   │
│   ├── config/                      # Configuration management
│   │   ├── __init__.py
│   │   └── config_manager.py        # Paths, logging, environment config
│   │
│   ├── bronze/                      # Bronze Layer - Raw Data Ingestion
│   │   ├── __init__.py
│   │   ├── data_loader.py           # Main bronze data loader
│   │   ├── csv_ingestor.py          # CSV customer data ingestion
│   │   └── xml_ingestor.py          # XML order data ingestion
│   │
│   ├── silver/                      # Silver Layer - Data Cleaning & Enrichment
│   │   ├── __init__.py
│   │   ├── silver_processor.py      # Main silver processor
│   │   ├── data_cleaner.py          # Data cleaning operations
│   │   ├── data_validator.py        # Data validation & quality checks
│   │   └── data_enricher.py         # Feature engineering & enrichment
│   │
│   ├── gold/                        # Gold Layer - Business Intelligence
│   │   ├── __init__.py
│   │   ├── gold_processor.py        # Main gold processor
│   │   ├── kpi_calculator.py        # Core KPI calculations
│   │   └── business_metrics.py      # Additional business metrics
│   │
│   ├── presentation/                # Visualization & Reporting
│   │   ├── __init__.py
│   │   ├── visualizer.py            # Business dashboard generation
│   │   └── report_generator.py      # Text and JSON report generation
│   │
│   └── utils/                       # Utility functions
│       ├── __init__.py
│       ├── database.py              # Database connection & operations
│       └── helpers.py               # Common helper functions
│   
│
└── docs/                            # Documentation
```
