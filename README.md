# Superstore Transaction Analysis
### Feature Engineering (RFM)

This project uses data from Tableau Public on Customer transactions to compute RFM (Recency, Frequency, Monetary Value) and then segment customer orders through kmeans clustering.
The data can be found and downloaded here: 
- https://community.tableau.com/s/contentdocument/0694T000001GnpUQAS

For this project, we download the data from a link made available through University of Washington (https://library.startlearninglabs.uw.edu/DATASCI420/2019/Datasets/SuperstoreTransaction.csv).

#### Abstract

Our data consists of \~10,000 products bought in ~5,000 orders made by ~800 customers from 2014-2017.  Our goal is to engineer new features to inform customer segmentation for promotional targeting.

Specifically, we aggregate product purchases to customer orders and compute RFM, then (kmeans) cluster those orders based on our new quantitative features measuring recency, frequency, and value.
