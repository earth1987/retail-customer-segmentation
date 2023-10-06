# Retail customer segmentation

The aim of this project is to conduct customer segmentation using a clustering algorithm. This will involve dividing a diverse customer base into smaller, homogeneous groups based on shared characteristics like demographics, behavior, or preferences. 

**Why?**

This strategy is invaluable as it enables businesses to tailor their marketing efforts, products, and services to each segment's specific needs and preferences. By doing so, companies can enhance customer satisfaction, loyalty, and profitability. Moreover, it allows for more efficient resource allocation, helping businesses focus their resources where they are most likely to yield the highest returns.

# Scope
The dataset has been downloaded from [Kaggle](https://www.kaggle.com/code/karnikakapoor/customer-segmentation-clustering) It contains customer information collected from a mall's membership cards. As the data types are mixed, clustering will be tested using k-means (after one hot encoding), k-prototypes and hierarchical clustering (coupled with Gower's distance).

## File structure
<pre>
|- notebooks/
   |- data_exploration.ipynb
   |- model_selection_evaluation.ipynb
   |- figures/
|- retail-customer-segmentation/
   |- custom_funcs.py
   |- config.py
|- data/
   |- raw/
   |- cleaned/
|- README.md
</pre>

## Conclusion
Clustering was most effective with the k-prototypes algorithm. This revealed the presence of five distinct clusters (described below). The algorithm successfully distringuished low income/spend groups according to age and spending patterns.

* Cluster 0 = Below average spend (lowest), income (lowest) and age (lowest). Above average no. of deal purchases. Below average no. of catalogue, store and web purchases. Despite low spend, above average no. of web visits (highest). Unlikely to be a parent. 

* Cluster 1 = Below average spend (just) and income. Above average age (highest). Above average no. of deal purchases (highest). Roughly average no. of store and catalogue purchases. Above average no. of web site visits and purchases. More likely to be a parent.

* Cluster 2 = Below average spend, age and income. Below average number of deal purchases. Below average no. of catalogue (lowest), store and web purchases. Despite low spend, above average no. of web visit. Unlikely to be a parent. 

* Cluster 3 = Above average spend (highest), income (highest) and age. Below average no. of deal purchases (lowest). Above average catalogue (highest), web (highest) and store (highest) purchases. Unlikely to have a child.



