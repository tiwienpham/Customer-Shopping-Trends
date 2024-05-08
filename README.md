![Header_1004801546_900x400_1119](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/c8809192-002f-469e-9292-e03291787ba1)
# CUSTOMER SHOPPING TRENDS ANALYSIS
## Introdution
Welcome to the repository for the Customer Shopping Trends Analysis project! In this project, the objective is to analyze customer shopping trends in a store by visualizing data and gaining insights into customer behavior and preferences.

The project involves leveraging various data visualization techniques to explore and interpret customer shopping data. By analyzing this data, we can uncover patterns, trends, and correlations that provide valuable insights for businesses in understanding their customers and making informed decisions.

In addition to utilizing data visualization techniques, the Customer Shopping Trends Analysis project also incorporates machine learning algorithms to cluster customers based on their shopping behavior and preferences. Clustering helps group customers with similar characteristics together, enabling businesses to gain a deeper understanding of different customer segments and adjust their marketing strategies accordingly.
## Objectives
- Understand Customer Behavior: The project seeks to gain insights into customer shopping behavior, including their preferences, purchase patterns, and trends. By analyzing customer data, we aim to uncover valuable information about what motivates customers to make purchases, their preferred products or categories, and their shopping frequency.
-	Identify Customer Segments: Through clustering techniques, the project aims to identify distinct customer segments based on their shopping behavior.
## Repository Structure
This repository is organized as follows:
- shopping_trends_updated: This directory contains the dataset used for project.
- Customer Shopping Trends: This directory contains Jupyter notebooks that walk through the various stages of the project, including data exploration, preprocessing, visualize data and model development.
- README.md: This file provides an overview of the project, its objectives, and instructions on how to use the repository.
## About Dataset
![Data](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/22806850-6a06-46dd-a4b4-8d1e1df82ead)
The Customer Shopping Trends dataset is a collection of data that captures various aspects of customer behavior and preferences related to shopping. It includes information such as age, gender, purchase amount, preferred payment methods, frequency of purchases, and feedback ratings. The dataset can be accessed from the following Kaggle URL: https://www.kaggle.com/datasets/iamsouravbanerjee/customer-shopping-trends-dataset. 

This dataset encompasses various features related to customer shopping preferences, gathering essential information for businesses seeking to enhance their understanding of their customer base. The dataset includes attributes such as:
- Customer ID - Unique identifier for each customer
- Age - Age of the customer
- Gender - Gender of the customer (Male/Female)
- Item Purchased - The item purchased by the customer
- Category - Category of the item purchased
- Purchase Amount (USD) - The amount of the purchase in USD
- Location - Location where the purchase was made
- Size - Size of the purchased item
- Color - Color of the purchased item
- Season - Season during which the purchase was made
- Review Rating - Rating given by the customer for the purchased item
- Subscription Status - Indicates if the customer has a subscription (Yes/No)
- Shipping Type - Type of shipping chosen by the customer
- Discount Applied - Indicates if a discount was applied to the purchase (Yes/No)
- Promo Code Used - Indicates if a promo code was used for the purchase (Yes/No)
- Previous Purchases - The total count of transactions concluded by the customer at the store, excluding the ongoing transaction
- Payment Method - Customer's most preferred payment method
- Frequency of Purchases - Frequency at which the customer makes purchases (e.g., Weekly, Fortnightly, Monthly)
## Data Preparation.

**1. Import Libraries.**

![Screenshot 2024-05-08 100627](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/9675a2cf-e067-48ef-bd04-fc0dc2542f97)
**2. Data frame information**

![Screenshot 2024-05-08 100739](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/7c075906-67ce-4f50-a0ab-5b0727e74eda)
**3. Checking missing value.**

![Screenshot 2024-05-08 101041](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/be3f9d0c-aab1-4a75-8d31-01fc562b6e9a)
**4. Checking duplicated data**

**5. Descriptive statistics data**

![Screenshot 2024-05-08 101309](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/6cb409f3-3bef-4a09-8d66-4ef2c2b6aa53)
## Data Exploration
**1. Number Customer by Gender**

![Number Customer by Gender](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/7491e6b7-86f0-4095-a81c-a44f5636ecae)
The majority of the customers are male, accounting for 68% of the total customer base. The remaining portion consists of female customers, representing 32%. The chart illustrates a noticeable disparity between male and female customers. This difference may be attributed to several factors, such as the data being collected from a men's fashion store. 

To attract more customers, store can develop new products that cater to the specific needs and preferences of each gender.  For instance, the company could offer products with colors, styles, or features that align with the preferences of male and female customers, respectively.

**2. Age Distribution**

![Age Distribution](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/d8d0d092-e719-4dc2-afa5-5b6450ee23c8)
Based on the age distribution chart, it can be observed that the customer base of the store is evenly distributed across all age groups from 20 - 70, indicating diversity within the customer base. 

However, to assess business effectiveness by age group and determine the age group that generates the highest revenue, it is necessary to combine further analysis with the **"Total Purchase Amount by Age Group"** chart.

**3. Total Purchase Amount by Age Group**

![Total Purchase Amount by Age Group](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/eb2f4c3e-ae86-4ba5-9512-72c34cc99760)
In this chart, I divided the customers into four age groups: 20-35, 35-50, 50-65, and over 65. From the chart, it can be seen that the first three age groups are likely to generate more revenue for the store, while the over 65 age group generates lower revenue. This may be due to the following reasons:

- **Age Group 20-35:** This age group has a high income, diverse shopping needs, and a tendency to keep up with the latest trends. They also tend to shop online more, Stores should develop more of their products on e-commerce platforms to attract more customers in this group.

- **Age Group 35-50:** This age group has stable careers, high income, and is willing to spend on quality products. They are also a potential customer segment for premium products.

- **Age Group 50-65:** This age group tends to be more frugal in their spending, shopping cautiously, and less responsive to marketing campaigns. Store need to have appropriate approaches to reach and attract this customer segment.
  
- **Age Group over 65:** This age group has lower income, limited spending capacity. Store need to consider offering products that align with the needs and affordability of this customer segment.
  
**4. Purchase Amount of Customer by Category**
  
![Purchase Amount of Customer by Category](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/7b242220-dd36-4223-a3c1-d22de0c425f3)
  From the chart, it can be observed that the majority of customers make purchases in the "Clothing" category, accounting for approximately 44.7% of the total customer base. This indicates that the store's clothing products are successfully attracting the target customer segment. The store should continue to invest in expanding and improving its clothing offerings to maintain customer satisfaction and attract new customers. The "Footwear" and "Accessories" categories also hold significant proportions, accounting for 31.8% and 15.5% respectively. This suggests that the store's footwear and accessory choices are also appealing to customers. The "Outerwear" category has a relatively small proportion of 7.9%%. This indicates that the store's outerwear products may not be as popular as other categories. Therefore, the store should regularly update styles and implement various marketing strategies to attract more customers to this product category.

However, customer distribution across categories may change depending on the season. So I conducted an analysis of **Seasonal Purchase Amount by Category**.

**5. Total Purchase Amount (USD) by Category and Season.**

![Total Purchase Amount (USD) by Category and Season](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/a787af44-8f1e-4629-94d0-8837ff41f5bb)
Overall, the chart shows that the Fall season has the highest shopping volume among customers, with higher total revenue compared to other seasons. This could be due to several reasons:

**- Pleasant weather:** Fall brings mild and pleasant climate, stimulating the demand for shopping for clothing, accessories, and other weather-appropriate products.

**- Outdoor activities:** Fall is often associated with outdoor activities such as traveling, camping, etc., creating a need for purchasing products suitable for these activities.

**- Shopping events:** Some major shopping events often take place in the Fall, such as Black Friday, Cyber Monday, etc., attracting a large number of shoppers.

**Analysis by Category**

**- Accessories:**
The highest demand for accessories is in the Summer-Fall season due to the hot weather, prompting people to accessorize themselves with items like hats, caps, sunglasses, etc. Alternatively, it could be because during this season, customers tend to travel more, so they equip themselves with accessories to enhance their outfits.

**- Clothing:**
The demand for clothing is evenly distributed across all four seasons, but the highest season is Spring. This is because it is a season with warm weather, prompting people to change their fashion style with light and breezy outfits. Additionally, the Winter season is also a time when customers shop for clothing more, as the cold weather requires additional items like coats, sweaters, etc.

**- Footwear:**
The majority of footwear purchases are made in the Summer-Fall season. Similar to accessories, during the Summer-Fall season, people tend to travel and engage in more outdoor activities, creating a higher demand for footwear.

**- Outerwear:**
The highest demand for outerwear is in the Fall-Winter season since it is a transitioning period into the cold Winter season, prompting people to acquire warm coats to prepare for the colder weather.

**6. Total Purchase Amount by Item Purchased.**

![Total Purchase Amount by Item Purchased](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/ae40e86d-0c28-43d9-ae09-d6784c9559a3)
Based on the chart, customers tend to purchase items such as Blouse, Shirt, Dress, Pants, Jewelry, and Sunglasses. This indicates their interest in fashion items like clothing and accessories. These products might be popular or trendy in your store.

To capitalize on this, store can enhance their marketing and advertising strategies by focusing on promoting these types of products, offering special deals or discounts, or even expanding your product line to meet the growing demand for these items. Additionally, maintaining product quality and service excellence is crucial to retaining existing customers and attracting new ones.

**7. Purchase Amount by Shipping Type and Purchase Amount by Payment Method**

![Purchase Amount by Shipping Type   Purchase Amount by Payment Method](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/81b28d46-55cf-4273-98c4-6432e08a1ab8)
**- Purchase Amount by Shipping Type**

The chart shows that Free Shipping and Express are the two most popular shipping methods, accounting for 17.5% and 16.8% of the total number of purchases, respectively. Therefore, the store should continue to offer the Free Shipping method to attract customers. In addition to the aforementioned shipping methods, the store may consider promoting expedited shipping options such as 2-hour delivery, same-day delivery, 2-Day Shipping, Next Day Air, or International Shipping to meet the diverse needs of customers. Besides providing a variety of shipping options, the store can collaborate with shipping companies to offer more competitive prices to customers and provide clear information about delivery times for each shipping method so that customers can choose the one that suits their needs.

**- Purchase Amount by Payment Method**

The chart shows that Credit Card is the most payment method, accounting for 17.3% of the total number purchases. It is followed by PayPal with a rate of 17.2% and Cash with a rate of 17.2%. In addition to these methods, the store can consider adding different payment options such as: Mobile Wallet or Buy Now, Pay Later to meet the diverse needs of customers. The store can provide promotional programs for customers using specific payment methods, for example implementing a 2.5% for prepaid transactions, or low-interest rates for After payments. Besides offering diverse of payment methods, the store have to always ensure the safety of payments transactions by using advanced security measures.

**8. WordCloud about Colors Trends.**

![WordClound of number color](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/14e1e311-1415-4c9c-b361-ce6ed01b0762)
From the WordCloud chart depicting the color trends chosen by customers,  that colors such as Yellow, Olive, Silver, Teal, Black, etc., are the preferred choices. This suggests certain color preferences or fashion trends among customers.

Understanding these color preferences can inform inventory management, product selection, and marketing strategies. For instance, store might emphasize items in these popular colors, create themed collections or promotions, or incorporate trending colors into their future product designs. Additionally, it can help you better tailor their offerings to meet the evolving tastes and preferences of their customer base.

**9. Top 10 Locations with Highest Purchase Amount (USD).**

![Top 10 Locations with Highest Purchase Amount (USD)](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/da459860-5806-4ef4-9e1c-b8eba28eea04)
From the Top 10 Locations with Highest Purchase Amount chart, we can observe that Montana is the region that generates the highest revenue, followed by Illinois, California, and Idaho, which also contribute significantly to the revenue. The store should focus on the high-revenue areas to increase sales. To continue increasing revenue, stores should collect and analyze customer data to better understand their preferences, needs, and shopping behaviors. This data can be used to develop more targeted and effective marketing campaigns. Additionally, the store should utilize multi-channel marketing to reach potential customers in various locations, such as social media, email marketing, online advertising, etc. Collaborating with influencers on social media in different regions can also help promote products to a large number of potential customers.

## Clustering.

**1. StandardScaler data.**
**2. Using the elbow method to optimize clustering.**

![Inertia analysis according to parameter k](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/0952fcf5-8140-4633-b82d-fdad0671d0ef)
Using the Elbow method to determine the optimal number of clusters and obtaining 4 as the result.

Elbow Method: The Elbow method is a popular technique for determining the optimal number of clusters in data clustering. It works by calculating the Within-Cluster Sum of Squares (WCSS) for each choice of the number of clusters and then plotting it on a graph. A point of inflection on the graph is typically where the decrease in WCSS begins to slow down, and the number of clusters corresponding to this point is often considered the optimal number of clusters.

**3. Using KMeans to Cluster.**

![Screenshot 2024-05-08 104006](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/51fdd859-aed2-417f-9e25-381ccce3c7b7)
## Cluster Visualization.

**1. Cluster Visualization based on Previous Purchases and Purchase Amount.**

![Cluster Visualization based on Previous Purchases and Purchase Amount](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/e41dd30b-39f5-4926-919a-02be1c64226f)
**2. Cluster Visualization based on Age and Purchase Amount.**

![Cluster Visualization based on Age and Purchase Amount](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/c4f4f2c8-6c43-4871-9ed9-e59fd27e3a56)
**Customers aged 20-45 with high spending power (Cluster 0):**
This is a group of customers with high potential for purchasing and could be a significant part of sales revenue. Therefore, the store needs to focus on providing high-quality products and services to maintain and strengthen relationships with this group. Consider enhancing online marketing strategies to reach and attract this customer segment.

**Customers over 45 years old with high spending power (Cluster 1):**

This group can be a stable customer base with high purchasing power. Special marketing strategies and promotions should be implemented to attract and retain this customer group. Provide good customer service to maintain long-term relationships and increase sales volume.

**Customers aged 20-45 with moderate to low spending power (Cluster 2):**

This could be a potential customer group for development but currently has limited spending. Create discount strategies, special offers, or lower-priced products to attract and retain this group. Develop membership programs or promotions specifically for this group to motivate additional purchases.

**Customers over 45 years old with moderate to low spending power (Cluster 3):**

This group could be price-sensitive customers and may require persuasion to spend. Create attractive discount strategies and offers to attract and retain customers in this group. Enhance promotion of products with prices suitable for this customer segment.

**3. Cluster Visualization based on Review Rating and Purchase Amount.**

![Cluster Visualization based on Review Rating and Purchase Amount](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/7ae2ecf9-cdc1-47e0-8172-09d17e13edfc)
## Conclusion.

Customer shopping trends analysis is a crucial tool that helps businesses gain a better understanding of consumers and provide effective marketing strategies. From data and charts, important conclusions can be drawn about customer groups and their shopping behaviors. Understanding customer shopping trends is the key to developing effective marketing strategies and optimizing sales revenue. By focusing on specific customer groups and meeting their needs, businesses can enhance customer relationships and achieve success in an increasingly competitive market.

![images](https://github.com/tiwienpham/Customer-Shopping-Trends/assets/119265751/fd1f0d97-94aa-4410-9ae9-f9b7b67802c9)


