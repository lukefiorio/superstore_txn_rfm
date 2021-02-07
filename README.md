# Superstore Transaction Analysis
### Feature Engineering (RFM)

This project uses data from Tableau Public on Customer transactions to compute RFM (Recency, Frequency, Monetary Value) and then segment customer order days through kmeans clustering.
The data can be found and downloaded here: 
- https://community.tableau.com/s/contentdocument/0694T000001GnpUQAS

For this project, we download the data from a link made available through University of Washington (https://library.startlearninglabs.uw.edu/DATASCI420/2019/Datasets/SuperstoreTransaction.csv).

### Abstract

Our data consists of \~10,000 products bought in ~5,000 orders made by ~800 customers from 2014-2017.  Our goal is to engineer new features to inform customer segmentation for promotional targeting.

Specifically, we aggregate product purchases to customer order days and compute RFM. We then cluster those orders based on our new quantitative features measuring recency, frequency, and value.  Building off of our RFM analysis we finish by incorporating those measure into a customer segmentation scheme.

### Results

Through RFM and kmeans clustering, we identified four customer segments.

**<ins>*Unprofitable Discount hunters*</ins>**
- The smallest cluster (11% of customers).  Defining characteristics: These customers buy products on massive discount (42% off, on average) and are extremely unprofitable as a result (-26% profit margin). They purchase relatively infrequently, but spend big (and save big) when they do.

**<ins>*Home-office shoppers*</ins>**
- A relatively small cluster (17% of customers).  Defining characteristics: These customers shop exclusively in the home-office segment; beyond that they are fairly typical.

**<ins>*High value customers*</ins>**
- A mid-sized cluster (25% of customers).  Defining characteristics: These customers shop often and spend the most.  They represent 63% of company profit, while only 25% of customers.

**<ins>*Core customers*</ins>**
- The biggest cluster (47% of customers).  Defining characteristics: Nearly half of customers, this group represents  typical shopping behavior.  They shop less often and tend to make smaller purchases when they do. While not the biggest spenders, they still turn a healthy profit (34% of total).

![Cluster Summary](images/superstore_cust_segment_profile.png?raw=true "Cluster Summary")

### Conclusion

Through our customer transaction analysis we were able to understand trends in overall sales, identify different types of transactions (through RFM), and segment customers into groups with distinct needs.

As with most analyses, this project should act as a strong starting point from which to kick off targeted campaigns and research.  We outline potential opportunities, concerns, and next steps for each customer segment below.

**<ins>*High value customers*</ins>**<br>
We found that 25% of our customers are extremely engaged and generating most of our profits.  Our main goal with these customers is retention.  Increased personalization and loyalty rewards will be key to keeping this group engaged.  Next steps for this group are to evaluate trends in engagements. We can use our wealth of transaction data with these customers to send personalized communications and promotional offers at the right time to stay top of mind and show that we value of them.  In the long-term, we should look to build a loyalty program around the needs and preferences of these customers.

**<ins>*Core customers*</ins>**<br>
Core customers make up half of our customer base.  They generate healthy profit, but don't purchase too frequently.  With this segment, we should be looking to foster growth and build stronger customer relationships. Our goal is to migrate these customers up the value chain into the *high value customers* segment.  Next steps for these customers are to understand purchase patterns and offer NPTB (next-product-to-buy) suggestions to encourage repeat visits and purchases.

**<ins>*Home-office shoppers*</ins>**<br>
While slightly more engaged than our core customer base, these customers are primarily unique in that they are specific to the home office segment.  Understanding trends in home office product sales can help inform how we communicate with these customers going forward.  Next steps may include further sub-segmentation of this closer to focus our efforts. 

**<ins>*Unprofitable Discount hunters*</ins>**<br>
This segment is relatively small - about 10% of our customers - but put a heavy tax on our bottom line.  Our goal with these customers is to either migrate them to profitability or disincent loss-leading purchases.  Placing tighter controls around which promotions are advertised to which customer segments, should be a quick win in boosting profitability with this group.
