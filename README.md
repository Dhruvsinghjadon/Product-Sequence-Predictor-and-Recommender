# Product-Sequence-Predictor-and-Recommender
## Libraries Used
| Library | Function |
| --- | --- |
| numpy | To manipulate the data |
| pandas| To manipulate the data|
| matplotlib |For data visualization |
| seaborn| For data visualization |
| mlxtend| For association rule mining |
| fastapi | For creating API |
| uvicorn | 	For model deployment |
| streamlit| To build the UI |
| requests | To connect the UI with the API |

## Data Source Used

This is a Brazilian ecommerce public dataset of orders made at Olist Store. The dataset has information of 100k orders from 2016 to 2018 made at multiple marketplaces in Brazil. Its features allows viewing an order from multiple dimensions: from order status, price, payment and freight performance to customer location, product attributes and finally reviews written by customers. There is also a geolocation dataset that relates Brazilian zip codes to lat/lng coordinates.

This dataset was generously provided by Olist, the largest department store in Brazilian marketplaces. Olist connects small businesses from all over Brazil to channels without hassle and with a single contract. Those merchants are able to sell their products through the Olist Store and ship them directly to the customers using Olist logistics partners.

After a customer purchases the product from Olist Store a seller gets notified to fulfill that order. Once the customer receives the product, or the estimated delivery date is due, the customer gets a satisfaction survey by email where he can give a note for the purchase experience and write down some comments.
## Churn Analysis
After performing Churn Analysis on the database, we infer that 97% of the customers churn out of the system, i.e., they make only one purchase in the entire lifetime of their purchase history. However, since the dataset has 10,00,000 data entries, we still have 3,000 entries to analyze.

## Database Schema

![Project recomand](https://user-images.githubusercontent.com/75934644/178632262-2b5fe4c4-94e7-4929-a072-bc1345654412.png)
 ## Conclusion & Future Work

The API works accurately, however, takes a lot of time to render the output owing to the large size of the dataset, time complexity of generating association rules and building the chain. When deployed on a larger scale, the working of the algorithm can be parallelized to improve the time efficiency and achieve micro-second response. Also, the database can be dynamically updated to store the entries of the new purchases made by the customer, which may lead to changes in the chain of products and cross-category sales.
