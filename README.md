# Association Rule Mining
Business Problem: “Global Mart” online store is an online store that caters to customers from across the globe. As the marketing manager of the store, you want to figure out the most frequently occurring combination of the items that are bought together. This would enable you to recommend the related items to a customer, once he makes a purchase in the store. 

As you would see, each row of the dataset represents an item of the order. However, the Order ID is not unique. Thus, the different items ordered at a time figure in different rows with the same Order ID. The number of unique products is too large a number to provide meaningful insight. Thus, the most relevant attribute to analyse would be the "Sub-Category" of the products.
 
Data Preparation
You have already seen that market basket analysis can be done on the transaction level data, where each row represents the items that are bought in a single transaction. To be able to use the "arules" package for association rule mining, you need to convert your data into transactions format. For that, you can either use as() function or read.transactions() function. It is advisable that you explore both these functions and their requirements and utility before proceeding further.
 
Data Mining & Evaluation
Once, you have the transaction level data, where each row represents the items bought in a single transaction, you can explore the association rules from the data using apriori principle. Here you would want to find the most business-relevant association rules, while also maximising the support, confidence or lift. You can also put a cap on your transactions by considering only those which have more than a threshold itemsets.
