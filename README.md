# **Product Ratings & Future Sales Analysis**

## **Project Overview**
This One Question Project examines whether product ratings can serve as an indicator of future sales performance. Rather than comparing ratings with lifetime sales, the analysis uses historical product ratings at a given point in time and compares them with sales generated in the following period. By analyzing products across rating groups, the project evaluates whether highly rated products consistently achieve higher future sales and whether customer feedback can provide a useful signal for future product performance.

## **Business Problem**
Product ratings are often used as a signal of customer satisfaction and product quality, but a high rating does not necessarily mean a product will perform well in the future. Businesses need to understand whether positive customer feedback can provide an early indication of future sales performance. Without this insight, ratings may be viewed only as a measure of past customer experience rather than a potential signal for future demand. This analysis investigates whether products with higher historical ratings generate stronger sales in subsequent periods, helping determine whether product ratings can be used as a meaningful indicator of future sales performance.

## **Project Goal**
The goal of this project is to determine whether historical product ratings are associated with higher future sales. The analysis will group products based on their ratings at a given point in time, compare their sales performance in the following period, and evaluate whether higher-rated products consistently achieve stronger future sales. The project aims to assess whether product ratings can serve as a useful leading indicator of future product performance.

## **Dataset Description**
The project uses three datasets representing product information, customer rating activity, and product sales performance over time.

**products.csv**<br>
Contains basic product-level information.

| Column        | Description                        |
| ------------- | ---------------------------------- |
| `product_id`  | Unique identifier for each product |
| `category`    | Product category                   |
| `price`       | Product selling price              |
| `launch_date` | Date the product was launched      |

**product_ratings.csv**<br>
Contains individual customer rating events for products.

| Column        | Description                             |
| ------------- | --------------------------------------- |
| `product_id`  | Unique identifier for the rated product |
| `rating_date` | Date the rating was submitted           |
| `rating`      | Customer rating from 1 to 5             |

**product_sales.csv**<br>
Contains daily sales performance for each product.

| Column       | Description                            |
| ------------ | -------------------------------------- |
| `product_id` | Unique identifier for the sold product |
| `sales_date` | Date the sales occurred                |
| `units_sold` | Number of units sold                   |
| `revenue`    | Revenue generated from product sales   |

## **Dataset Scope**
The three datasets are linked through `product_id`. The analysis uses historical rating activity to calculate each product's rating at a specific point in time, then compares it with sales generated in the following period. This allows the analysis to evaluate whether products with higher historical ratings tend to achieve stronger future sales performance.

## **Business Question**
### **Do product ratings predict future sales ?**