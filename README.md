# Community Detection & Recommendation System on E-Commerce Purchase Network

Final Project – Social Network Analysis

## Overview
This project analyzes consumer purchasing patterns in e-commerce using Social Network Analysis (SNA).

Transaction data is modeled as a product co-purchase network where:
- Nodes represent products
- Edges represent products purchased together

The Louvain community detection algorithm is used to identify clusters of products frequently bought together. These communities are then used to build a community-based product recommendation system.

This approach helps reveal hidden relationships between products and generate more relevant recommendations compared to global popularity-based methods.

---

## Project Workflow
1. Data Collection  
2. Data Preprocessing  
3. Product Co-Purchase Network Construction  
4. Community Detection (Louvain Algorithm)  
5. Network Visualization  
6. Community-Based Recommendation System  

---

## Dataset
The dataset contains e-commerce transaction records with attributes such as:

- InvoiceNo – Transaction ID  
- StockCode – Product ID  
- Description – Product name  
- Quantity – Number of items purchased  
- InvoiceDate – Transaction date  
- UnitPrice – Product price  
- CustomerID – Customer identifier  
- Country – Customer location  

Original dataset size: **541,909 rows**  
Sample used in this project: **500 unique transactions**

---

## Methodology

### Data Preprocessing
- Remove duplicate data
- Handle missing values
- Filter relevant transactions
- Format attributes for analysis

### Network Construction
A product co-purchase graph is created where:
- Nodes = Products
- Edges = Products bought in the same transaction
- Edge weight = Frequency of co-purchase

### Community Detection
Community detection is performed using the **Louvain algorithm**, which optimizes modularity to identify clusters within the network.

### Recommendation System
Product recommendations are generated based on:
- Products within the same community
- Products with strong co-purchase relationships

---

## Technologies Used
- Python
- Google Colab
- Pandas
- NetworkX
- Matplotlib
- Community-Louvain

---

## Key Insights
- Products form natural communities based on consumer purchasing behavior.
- Some products act as hub nodes connecting multiple communities.
- Community-based recommendations provide more contextual suggestions.

---

## Course
Social Network Analysis  
Telkom University Surabaya

---

## Authors
- Aura Aulia Anastasya Hadi Putri  
- Giselle Annisa Haffaf  
- Angel B. Tarigan  
- Ryanta Melinda S.

---

## License
This project is created for academic purposes as part of a university course assignment.
