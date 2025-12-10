# Final Project — Group 97  
**Social Graphs & Interactions**

This repository contains the complete codebase and data processing pipeline for the final project of **Group 97** in the course *Social Graphs & Interactions*.  
The project focuses on building, analyzing, and interpreting an actor collaboration network based on movie data, community detection, and sentiment analysis.

---

## Project Overview

The project is structured around three main components:

- **Network construction** from movie cast data  
- **Community detection and interpretation** using the Louvain algorithm  
- **Sentiment analysis** based on movie reviews using the LabMT lexicon  

The goal is to uncover structural properties of the actor network, identify important actors and communities, and analyze how sentiment varies across different parts of the network.

---
## Data Sources

The project uses the following data sources:

- Movie overview and metadata (MovieLens-style datasets)
- Movie reviews fetched from the **TMDB API**
- **LabMT happiness lexicon** for sentiment analysis

---


---

## Main Analysis Components

### 1. Data Preparation and Network Construction
- Cleaning cast and genre data
- Filtering movies by genre
- Constructing a weighted actor collaboration network
- Removing isolated nodes

### 2. Centrality Analysis
- Degree centrality
- Betweenness centrality
- Eigenvector centrality  
Used to identify the most influential actors in the network.

### 3. Community Detection
- Extraction of the Giant Connected Component (GCC)
- Louvain community detection
- Modularity evaluation
- Community hub detection and automatic naming

### 4. Community Interpretation
- Aggregation of movie overviews per community
- TF–IDF keyword extraction for thematic labeling

### 5. Sentiment Analysis
- Review-level sentiment using the LabMT lexicon
- Aggregation from reviews → movies → actors → communities
- Ranking communities by average sentiment

### 6. Backbone Extraction
- Disparity Filter applied to reduce network complexity
- Visualization of the backbone structure

---

## Repository Structure

```text
.
├── explainer.ipynb          # Jupyter Notebooks for analysis
├── images/                  # Generated plots and network visualizations
├── README.md                # Project documentation
