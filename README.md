# Trending YouTube Videos Analysis Project

Welcome to the Trending YouTube Videos Analysis Project repository! This project combines data engineering, data analytics, and cloud to analyze YouTube video trends based on categories and metrics, providing key insights for further exploration and reporting.

## Overview

This project aims to:

- **Securely manage, streamline, and analyze YouTube data** to uncover trends.
- Combine structured and semi-structured data into actionable insights.
- Build a robust, scalable system leveraging cloud services.
- Provide interactive reporting for key performance indicators (KPIs).

## Project Goals

1. **Data Ingestion**: Implement a mechanism to securely and efficiently ingest data from different sources.
2. **ETL System**: Process raw data into a clean and analyzable format.
3. **Data Lake**: Centralized storage for multiple datasets in a single repository.
4. **Scalability**: Ensure the system can handle increasing data volumes.
5. **Cloud Integration**: Leverage AWS for scalable computing and data processing.
6. **Reporting**: Create dashboards for analyzing insights and delivering KPIs to end consumers.

## Architecture Diagram

<img src="architecture.jpeg">

## Technologies and Services Used

### **Amazon Web Services (AWS)**

- **Amazon S3**: Object storage for centralized and scalable data management.
- **AWS IAM**: Identity and access management for secure resource permissions.
- **AWS Glue**: Serverless service for data integration and transformation.
- **AWS Lambda**: Compute service for running code in a serverless environment.
- **AWS Athena**: Interactive query service for analyzing data directly from S3.

### **Other Tools**

- **Microsoft Power BI**: Used as the primary business intelligence tool for visualization and reporting.

## Dataset Used

We used a dataset from Kaggle, which contains statistics on daily popular YouTube videos across regions. It includes details such as:

- Video title, channel title, publication time, and tags.
- Views, likes, dislikes, and comment counts.
- Video description and category IDs.

Dataset link: [YouTube Trending Dataset](https://www.kaggle.com/datasets/datasnaek/youtube-new)

## Project Structure

- **/ETL_scripts**: Contains scripts for extracting, transforming, and loading data.
- **/S3_data_storage**: Configuration for Amazon S3 buckets.
- **/Glue_jobs**: Scripts and workflows for AWS Glue jobs.
- **/Lambda_functions**: AWS Lambda function scripts for automation.
- **/PowerBI_reports**: Power BI `.pbix` files for data visualization.
- **README.md**: Overview of the project.

## Getting Started

### Prerequisites

1. AWS account with access to S3, IAM, Glue, Lambda, and Athena.
2. Microsoft Power BI Desktop.
3. Basic understanding of SQL and cloud architecture.

### Steps to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/trending-youtube-analysis.git
   ```

2. **Data Ingestion**:

   - Upload raw datasets to the designated S3 bucket.

3. **ETL Process**:

   - Use AWS Glue to transform and clean the data.
   - Store the processed data in an organized S3 folder structure.

4. **Query Data**:

   - Use AWS Athena to run SQL queries on processed data stored in S3.

5. **Reporting**:
   - Load the queried data into Power BI.
   - Explore insights using interactive dashboards.

## Insights Provided

- **Trending Metrics**: Analysis of top-performing videos by region and category.
- **Engagement Analysis**: Trends in likes, dislikes, and comments.
- **Category Insights**: Performance of different video categories over time.

## Future Enhancements

- Implement real-time data ingestion using AWS Kinesis.
- Include sentiment analysis of video comments.
- Expand the dashboard to cover regional comparisons.
- Introduce correlation analysis between metrics such as views, likes, description, category, and comments to identify deeper relationships.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or collaboration, feel free to reach out:

- **Email:** alexandersolizar@gmail.com
- **GitHub:** [alexsolizar](https://github.com/alexsolizar)

---

We hope this project serves as a valuable resource for analyzing YouTube trends. Contributions are welcome!

## Credits

The methodologies used in this project is based on dataengineering-youtube-analysis-project repository of Darshil Pamar.
I have introduced some changes to fit with the use cases of this project.
