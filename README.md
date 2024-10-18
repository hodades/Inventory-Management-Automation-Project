# Inventory Management Automation Project

## Overview
This project is an automation solution developed to streamline inventory management processes using Make, an AI tool, and workflow automation. The solution integrates with Slack and utilizes data from Google Sheets to provide real-time updates and actionable insights to the inventory management team, reducing manual operations and increasing efficiency.

## Objective
The main goal was to centralize inventory information and coordinate team activities, ensuring smooth operations and avoiding duplication of efforts. The project focuses on automating stock management tasks, including:

- Monitoring stock levels.
- Sending notifications for restocking needs.
- Promoting new products and adjusting prices based on performance.
- Removing out-of-stock items from the website to enhance the customer experience.

## Features
1. **Slack Integration**: The application sends automated messages to the team, providing alerts and options for actions such as stock updates, website modifications, and advertising campaigns.
2. **Dynamic Insights**: Using data from Google Sheets, the application generates KPIs and insights that trigger Slack notifications through Make.
3. **Stock Management Automation**:
   - **Real-Time Monitoring**: Continuously tracks stock levels and generates alerts when restocking or product promotion is needed.
   - **Promotion Optimization**: Automatically identifies products to promote on the website and updates advertising campaigns accordingly.
   - **Price Management**: Adjusts product prices to optimize profitability based on performance metrics.

  ![image](https://github.com/user-attachments/assets/eaae9e8b-5a67-434d-a651-59cdbc582f1b)

## How to read the Google Sheet :
Certainly! Here's the English translation of the text you provided:

How to read the table (monthly period)
Let's analyze the product line with **ID: 13346**:
* **product_id: 13346**
* **category_1: Home**
* **category_2: Fashion**
* **category_3: Luggage**
* **price: 2.39** (unit price of the product)
* **new: 1** (this is a new product)
* **forecast_stock: 100** (forecasted stock quantity)
* **stock: 100** (current available stock quantity)
* **product_name: 13346-Home-Fashion-Luggage** (product name, here automatically generated with categories and ID)
* **STOCK VALUE: 239** (total value of current stock = 100 units x €2.39)
* **IN_STOCK: 1** (the product is in stock)

**Analysis:**
1. **New product**:
   * This product is marked as new (**new: 1**), which may mean it has been recently added to the inventory. It's a good candidate for marketing campaigns, website features, or promotional offers to attract customer attention.
2. **Current and forecasted stock**:
   * The **current stock** is **100 units**, and the **forecast stock** is also **100 units**. This indicates that the inventory is stable and no replenishment is currently planned, which may suggest that the company considers this stock level sufficient to meet current demand.
3. **Stock value**:
   * The **stock value** is **€239**. This represents the total value of the 100 units of this product currently available. This information is useful for assessing the financial impact of this product in the overall inventory and its relative importance in the range.
4. **Product in stock**:
   * The product is available for sale (**IN_STOCK: 1**). There is no risk of immediate stockout, which is reassuring if demand arises.

**Conclusion:**
Product 13346 seems well-stocked with 100 units in stock and a total value of €239. Being a new product, it might be relevant to promote it to ensure it sells well. No replenishment is necessary in the short term, but if demand increases, sales will need to be monitored to avoid a stockout.

Products to exclude:
For the product **ID 112481**, the values new = 0, forecast_stock = 0, and stock = 0 indicate that this product **is neither new nor currently available in stock**, and there **is no forecast for future demand**. It should be considered obsolete.

Expectations of the "inventory management" team
**1. Promotion of new products**
* **Goal**: Highlight new products on the site and create an advertising campaign.
* Application ads_manager & Site-ecommerce
**2. Out of stock**
* **Goal**: Remove out-of-stock items from the site to avoid customer frustration.
* Application Site-ecommerce
**3. Replenishment**
* **Goal**: Monitor and optimize stock levels. Indicate the quantity to replenish and why this choice?
* Application Supply_order

## Technologies Used
- **Make**: For data analysis, workflow automation, and generating recommendations.
- **Slack API**: For sending notifications and integrating with stock management workflows.
- **Google Sheets**: To centralize and analyze stock data.

## Deliverables
- A blueprint detailing the automated solution.
- Configured insights using custom formulas to create automatic triggers.
- A dedicated Slack channel to centralize team notifications and actions.

## Conclusion
This project implements an innovative solution for automating inventory management, reducing manual tasks, and improving operational efficiency through the use of Make and integrated workflows.
