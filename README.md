
# PySpark Fundamentals on NYC Taxi Ride Dataset

This project demonstrates core PySpark concepts and data engineering techniques using the New York City Taxi Ride dataset. The included Jupyter notebook provides a hands-on, well-documented walkthrough of distributed data processing, cleaning, and analysis with PySpark.

## Dataset [Download](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)
- **Source:** NYC Taxi Ride data (sample Parquet files and zone lookup CSV)
- **Files:**
	- `dataset/yellow_tripdata_2025-01.parquet`, `yellow_tripdata_2025-02.parquet`
	- `dataset/taxi_zone_lookup.csv`

## What You'll Learn

The notebook provides comprehensive coverage of PySpark fundamentals through hands-on examples:

### Core DataFrame Operations
1. **SparkSession Initialization** – Entry point for Spark functionality
2. **Data Loading** – Reading Parquet files and CSV efficiently
3. **DataFrame Inspection** – Exploring schema, columns, and summary statistics
4. **Data Selection** – Selecting and projecting specific columns
5. **Data Sorting** – Ordering data by one or more columns with custom sorting
6. **Data Filtering** – Subsetting data with complex conditions
7. **Data Cleaning** – Handling missing values and quality checks
8. **Feature Engineering** – Creating new columns (e.g., trip duration from timestamps)
9. **Column Renaming** – Standardizing column names for clarity
10. **Dropping Columns** – Removing unnecessary columns after transformations

### Data Combination & Aggregation
11. **Unions** – Combining DataFrames vertically (row-wise stacking)
12. **Joins** – Combining DataFrames horizontally (INNER, LEFT, RIGHT, OUTER)
13. **Grouping & Aggregation** – Summary statistics by category (count, sum, avg, min, max)
14. **Writing Data** – Saving results to CSV and other formats

### Advanced Topics
15. **SQL Operations** – Using Spark SQL with temporary views
16. **Complex Queries** – Combining SQL with DataFrame operations
17. **Production Considerations** – Scalability, reliability, and security requirements

### Hands-On Practice
18. **Challenge Exercise 1** – Complete data pipeline with unions, joins, and transformations
19. **Challenge Exercise 2** – SQL joins with aggregation for business analytics
20. **Real-world Scenario** – NYC taxi data analysis combining all concepts

### Advanced PySpark Topics (NEW!)
21. **Window Functions** – Running totals, rankings, and row comparisons
    - Examples: Running sums, row numbering, lag/lead functions
    - Challenge: Calculate moving averages with window functions

22. **Pivot Tables** – Multi-dimensional data summarization
    - Examples: Average fare by payment type and passenger count
    - Challenge: Create pivot tables with multiple aggregations

23. **User Defined Functions (UDFs)** – Custom Python functions for complex logic
    - Examples: Categorizing trips, flagging high-value transactions
    - Challenge: Create fare efficiency UDFs with custom scoring

24. **Data Quality & Outlier Detection** – Identifying anomalies and data issues
    - Examples: Z-Score and IQR methods for outlier detection
    - Challenge: Multi-condition quality scoring system

25. **Partitioning & Performance** – Optimizing storage and query performance
    - Examples: Single and multi-level partitioning strategies
    - Challenge: Design optimal partitioning for analytics

Each concept is explained with clear documentation, detailed comments, practical examples, and hands-on challenges. Every section builds progressively on previous knowledge.

## Getting Started

### Requirements
- Python 3.7+
- Jupyter Notebook or VS Code with Jupyter extension
- PySpark (install via `pip install pyspark`)

### Running the Notebook

### Quick Start
```bash
# Clone the repository
git clone <repository-url>
cd pyspark-fundamentals-on-NYCTaxiRide-dataset

# Install PySpark
pip install pyspark

# Start Jupyter
jupyter notebook
# or use VS Code with Jupyter extension
```

### Using the Notebook
1. Open `PySpark.ipynb` in Jupyter or VS Code
2. Run cells sequentially from top to bottom
3. Pay attention to the markdown explanations before each code section
4. Modify code and experiment with different approaches
5. Complete the challenge exercises to reinforce learning

### Dataset Files
- Place dataset files in the `/dataset` directory
- Required files:
  - `yellow_tripdata_2025-01.parquet`
  - `yellow_tripdata_2025-02.parquet`
  - `taxi_zone_lookup.csv`

## Notebook Structure

**Section 1: Fundamentals** (Cells 1-14)
- Overview and learning objectives
- SparkSession initialization
- Data loading from Parquet files
- DataFrame exploration (schema, columns, statistics)
- Basic transformations (select, filter, sort)
- Data cleaning and missing values
- Feature engineering with timestamps
- Column management (rename, drop)

**Section 2: Data Combination** (Cells 15-17)
- Union operations (combining rows)
- Join operations (combining columns with keys)
- Lookup table enrichment
- Practice exercises with complete solutions

**Section 3: Aggregation & Grouping** (Cells 18-22)
- Group by operations
- Aggregation functions (count, avg, sum)
- Meaningful aliases for columns
- Challenge exercises with detailed solutions

**Section 4: SQL & Advanced** (Cells 23-27)
- Creating and querying temporary views
- Complex SQL queries
- Combining SQL with DataFrame operations
- Challenge: SQL joins with aggregation
- Production environment considerations

**Section 5: Advanced Topics** (Cells 28-47) ⭐ NEW
- **Window Functions**: Running totals, rankings, and comparisons
- **Pivot Tables**: Multi-dimensional summarization
- **UDFs**: User-defined functions for custom logic
- **Outlier Detection**: Data quality and anomaly identification
- **Partitioning**: Performance optimization through smart storage

**Section 6: Summary** (Cells 48-49)
- Complete reference of transformations vs actions
- Performance optimization tips
- Best practices guide
- Next steps and advanced topics to explore

## 🚀 Next Steps & Advanced Topics

After mastering these fundamentals, continue your learning journey:

### Data Processing & Transformation
- **Window Functions**: OVER, PARTITION BY, ROW_NUMBER for analytics
- **Complex Joins**: Multi-condition joins, handling join skew
- **Advanced Aggregations**: rollup(), cube(), pivot() for multi-dimensional analysis
- **Custom Functions**: Building User Defined Functions (UDFs)

### Performance & Optimization
- **Data Partitioning**: Optimizing query performance through partitioning strategy
- **Caching & Persistence**: Memory management with .cache() and .persist()
- **Query Optimization**: Understanding Spark execution plans
- **Broadcast Variables**: Efficient handling of large read-only data

### Streaming & Real-Time Processing
- **Spark Structured Streaming**: Real-time data processing pipelines
- **Kafka Integration**: Consuming data from message brokers
- **Stateful Operations**: Window functions on streaming data

### Machine Learning
- **PySpark MLlib**: Classification, regression, clustering models
- **Feature Engineering**: Scaling, encoding, transformations
- **Model Evaluation**: Cross-validation, hyperparameter tuning
- **ML Pipelines**: Reproducible, production-ready workflows

### Advanced Data Engineering
- **Data Lakes**: Delta Lake, Apache Iceberg for ACID transactions
- **ETL Pipelines**: Building robust production data pipelines
- **Data Quality**: Validation, profiling, and anomaly detection
- **Schema Management**: Handling schema evolution

### Deployment & Operations
- **Cluster Deployment**: YARN, Kubernetes, cloud platforms
- **Job Scheduling**: Airflow, Oozie, cloud schedulers
- **Monitoring & Logging**: Performance tracking and troubleshooting
- **Cost Optimization**: Resource management and billing

### Integration & Ecosystem
- **Database Connectivity**: Integrating with SQL/NoSQL databases
- **Cloud Platforms**: AWS EMR, Google Dataproc, Azure HDInsight
- **BI & Visualization**: Exporting to Tableau, Power BI, etc.
- **Workflow Orchestration**: Complex multi-step data pipelines

