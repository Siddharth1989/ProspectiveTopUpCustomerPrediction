# ProspectiveTopUpCustomerPrediction
MonPG provides its loan services to its customers and is interested in selling more of its Top-up loan services to its existing customers. The goal was to identify the customers who are likely to purchase MonPG's top-up services in the future. I developed and persisted a SparkML pipeline model to identify potential customers that may purchase any Top-up services in the future (Part 1). Furthermore, I created a SparkML machine learning pipeline stream using Kafka and Spark Streaming using the persisted pipeline model (Part 2).<br>

**Note**: Part 2 of this project was implemented with the help of dedicated cloud servers at Monash University. These servers were used to start a new Kafka session. To reuse this code in your own environment, you may need to set up your own Kafka servers.

Dataset Information:<br>
1. Customer data contains variables related to basic service information. For example, frequency of the loan, tenure of the loan, disbursal amount for a loan & LTV.
2. The bureau data includes the behavioural and transactional attributes of the customers, such as current balance, loan amount, overdue, etc., for various tradelines of a given customer.<br>
3. Please refer to this link for more details on these datasets:
https://www.kaggle.com/datasets/rizdelhi/analytics-vidya-ltfs-finhack-3?select=ltfs3_train_bureau.csv
4. Please refer to the releases for the customer and bureau datasets.<br>

Part 1:<br>
 
1. I derived a new column called “Top-up” from the column called "Top-Up Month" as the label where (label 0 corresponds to No Top-up Service event, and label 1 represents all other types of Top-Up service).<br>
2. The series of steps that were performed to train the Spark ML model is given in the markdown sections of the part 1 notebook.<br>

Part 2:

1. The order execution for the Part 2 notebooks is Producer -> spark streaming -> Consumer.
2. Please refer to the markdown sections of the notebook for more information on the code.

Please use appropriate referencing as decreed under the GNU 3.0 public license to reuse the code or findings of this study in your work.
