# ProspectiveTopUpCustomerPrediction
MonPG provides its loan services to its customers and is interested in selling more of its Top-up loan services to its existing customers. We developed a SparkML model with a custom String Indexer to identify potential customers that may purchase any Top-up services in the future.<br>
Dataset Information:<br>
1. Customer data contains variables related to basic service information. For example, frequency of the loan, tenure of the loan, disbursal amount for a loan & LTV.
2. The bureau data includes the behavioural and transactional attributes of the customers, such as current balance, loan amount, overdue, etc., for various tradelines of a given customer.<br>
3. Please refer to this link for more details on these datasets:
https://www.kaggle.com/datasets/rizdelhi/analytics-vidya-ltfs-finhack-3?select=ltfs3_train_bur
eau.csv
4. Please refer to the releases for the customer and bureau datasets.<br>

Part 1:<br>

We derived a new column called “Top-up” from the column called "Top-Up Month" as the label where (label 0 corresponds to No Top-up Service event, and label 1 represents all other types of Top-Up service).<br>
Please use appropriate referencing as decreed under the GNU 3.0 public license to reuse the code or findings of this study in your work.
