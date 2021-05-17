# Conversion Paths of Google Merchandise Store Transactions

# Project Overview:

The objective of this project is to garner insights into the customer journey that led customers to purchase in the past30 days. It considers a 90-day conversion window to spot all the interactions (channel entry points) visitors have had with the e-commerce until placing their order - referred to as conversion path in this project.

Understanding the customer journey is valuable for business as they can know which communication touchpoints are bringing more revenue and how the company can enhance the channels that have the least contribution to the number of transactions and revenue.

# Data Description:

This project uses public data from Google Merchandise Store available as a sample in BigQuery. The data was partitioned into several sets by date, the table's records were granular at the visitor ID level, and the data used in this project included information on:

  - Traffic source (where website visitors come from) such as organic traffic, direct traffic, referral traffic, paid search traffic,etc. 
  - Transactional data: information about the transactions that occur on the Google Store website such as transaction ID, transaction revenue, transaction tax, etc. 
 
The data can be found <a href='https://console.cloud.google.com/bigquery?utm_source=bqui&utm_medium=link&utm_campaign=classic&project=practice-250123&ws=!1m9!1m4!4m3!1sbigquery-public-data!2sgoogle_analytics_sample!3sga_sessions_20170801!1m3!3m2!1sbigquery-public-data!2sgoogle_analytics_sample&d=google_analytics_sample&p=bigquery-public-data&page=dataset'>here</a>

# Technical Overview:

The approaches used to create and understand the conversion paths of the visitors included SQL and Python codes ran in Google Colaboratory. 

  - Retrieval of transactions that occurred in the last 30 days was captured (one-month window analysis);
  - Aggregation of data into first and last visits dates, and acquisition channel by visitor ID;
  - Retrieval of the transactions data such as transaction datetime and revenue by visitor;
  - Establishment of a 90-day lookback window to include only visits occurred as of that date interval and capture the conversion path for each transaction in the last 30 days       by visitor;
  - Calculation of the average ticket for the top 10 conversion paths by revenue and visualization of results;
  - Computation of number of transactions by conversion path;
  - Processing of top 10 transactions by length of conversion path;
  - Descriptive statistics of transactions revenue;
  - Plot of conversion paths by revenue. 

# Results: 

For the detailed results, please refer to this file: <a href:'https://github.com/aadamante/conversion_paths_sql_python/blob/main/Conversion_Paths_Analysis_Github_Version.ipynb'> Conversion_Paths_Analysis_Github_Version.ipynb </a>


