
# Customer Segmentation

### Task
- To do Exploratory Data Analysis on the given dataset
- Identify potential customer segmentation using RFM model
- Provide meaningful insights based on the above customer segmentation
- What action should the company take based on these insights
- List the champions, potential customers and customers who need attention.


### RFM model
RFM analysis gives marketers the ability to communicate with individual consumer clusters in a way that is much more appropriate for their unique behaviour.
This results in considerably greater response rates, as well as a boost in customer loyalty and lifetime value. An RFM model is a potent tool for identifying groups of clients who should receive particular treatment, much like other segmentation techniques. 
RFM, which stands for recency, frequency, and money.

While there are countless ways to perform segmentation, RFM analysis is popular for three reasons:

  - It utilizes objective, numerical scales that yield a concise and informative high-level depiction of customers.
  - It is simple – marketers can use it effectively without the need for data scientists or sophisticated software.
  - It is intuitive – the output of this segmentation method is easy to understand and interpret.

  Recency: How much time has elapsed since a customer’s last activity or transaction with the brand?

  Frequency: How often has a customer transacted or interacted with the brand during a particular period of time?

  Monetary: Also referred to as “monetary value,” this factor reflects how much a customer has spent with the brand during a particular period of time.


  ### Algorithm
For defining the RFM model we use the following attributes
- DAYSSINCELASTORDER  	 	 - Recency
- TOTAL_ORDERS 		         - Frequency
- REVENUE					 - Monetary Value


We define a score out of 3 for each of the above attributes.
This score is calculated by dividing the range of each attribute for all customers into 3 sections. Whichever section the particular customer belongs in he or she will be provided a score based on that. 
For Instance if customer A belongs in the third quartile in terms of frequency then customer A is provided a score of 3. 
The same applies to monetary value as well. 

For recency however, the lower the recency, the higher the score is provided as that indicates that the customer has recently purchased a product from the company.

Now that we have provided each customer a score out of 3 for recency, frequency and monetary value, to segment the customers we can use all these three scores and split them into different categories. 
We use the following categories- 

- Champions - Loyal Customers, who are the champions of all the customers with highest score of RFM.
- Loyalists-  Customers who have the most potential to become the Champions.  They recently buy the products and they make their purchases quite frequently but not expensive products
- Potential Customers - Customers whose frequency score and monetary score are slightly lower as they are newer customers who have recently shopped here
- Can’t Lose - Customers who used to pay a lot of money and come to the store frequently but they did not purchase recently. 
- At Risk- Customers who do not come to store often and not frequently make purchases.
- About to Sleep - Customers who haven't paid a visit to the store for a long time. However, once in a while, they do spend lot of money
- Need Attention- Customers who the company may lose out on



### Execution and results
Run the ipynb file. It consists of EDA as well as customer segmentation using RFM.

Data insights and company action for different customers are mentioned in the ppt named Presentation.

The Output folder contains three excel sheets each consisting of the customer IDs of the champions, potential customers and customers who need attention.
