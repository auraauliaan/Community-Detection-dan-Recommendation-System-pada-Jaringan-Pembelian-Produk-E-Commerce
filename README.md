Community Detection & Recommendation System on E-Commerce Purchase Network

Final Project — Social Network Analysis

Overview

This project analyzes consumer purchasing patterns in e-commerce using Social Network Analysis (SNA).

Transaction data is modeled as a product co-purchase network, where:

Nodes represent products

Edges represent products purchased together

The Louvain community detection algorithm is used to identify clusters of products that are frequently bought together. These communities are then used to build a community-based product recommendation system.

This approach helps reveal hidden relationships between products and generate more relevant recommendations compared to global popularity-based methods.

Project Workflow

Data Collection
↓
Data Preprocessing
↓
Product Co-Purchase Network Construction
↓
Community Detection (Louvain Algorithm)
↓
Network Visualization
↓
Community-Based Recommendation System

Dataset

The dataset contains e-commerce transaction records with the following attributes:

Feature	Description
InvoiceNo	Transaction ID
StockCode	Product ID
Description	Product name
Quantity	Number of items purchased
InvoiceDate	Transaction date
UnitPrice	Product price
CustomerID	Customer identifier
Country	Customer location

After preprocessing:

Original dataset: 541,909 rows

Sample used for analysis: 500 unique transactions

Methodology
1. Data Preprocessing

Removing duplicate records

Handling missing values

Filtering relevant transactions

Formatting attributes for analysis

2. Network Construction

A product co-purchase graph is created where:

Nodes = Products

Edges = Two products purchased in the same transaction

Edge weight = Frequency of co-purchase

3. Community Detection

Community detection is performed using the Louvain algorithm, which optimizes modularity to detect clusters within the network.

4. Network Visualization

The network is visualized to analyze:

central products (hub nodes)

cluster structures

relationships between product communities

5. Recommendation System

Product recommendations are generated based on:

products within the same community

products with strong co-purchase relationships

Example Recommendation

Input Product

RED WOOLLY HOTTIE WHITE HEART

Recommended Products

WHITE METAL LANTERN

WHITE HANGING HEART T-LIGHT HOLDER

CREAM CUPID HEARTS COAT HANGER

PINK HEART SHAPE COASTER

SET 7 BABUSHKA BOXES

These recommendations are based on actual co-purchase relationships in the network.

Technologies Used

Python

Google Colab

Pandas

NetworkX

Matplotlib

Community-Louvain

Project Structure
ecommerce-community-detection
│
├── data
│   └── ecommerce_transactions.csv
│
├── notebooks
│   └── community_detection_analysis.ipynb
│
├── images
│   └── network_visualization.png
│
├── src
│   └── recommendation_system.py
│
└── README.md
Key Insights

Products form natural communities based on consumer purchasing behavior.

Some products act as hub nodes connecting multiple communities.

Community-based recommendations provide more contextual suggestions for users.

Course

Social Network Analysis
Telkom University Surabaya

Authors

Aura Aulia Anastasya Hadi Putri

Giselle Annisa Haffaf

Angel B. Tarigan

Ryanta Melinda S.

License

This project was created for academic purposes as part of a university course assignment.
