
# Emotional Community Detection in Social Networks

This repository presents a project on **Emotional Community Detection in Social Networks**, a comprehensive system that utilizes sentiment analysis and community detection techniques to identify emotional communities within social media platforms like X (formerly Twitter). By exploring the interactions between users and their emotional expressions, this project offers insights into group behaviors and sentiment trends within online communities.

## Project Overview

Social media platforms have become essential tools for communication and public expression, generating vast amounts of data that provide a unique window into people's emotions and interactions. **Sentiment analysis** focuses on understanding user emotions through text, while **community detection** aims to uncover groups of users with stronger internal connections. Combining these techniques helps in discovering emotionally-driven communities, offering valuable insights for various applications like marketing, public opinion analysis, and misinformation detection.

### Key Objectives:
- Detect communities of users based on their emotional expressions.
- Analyze sentiment trends and their temporal evolution.
- Visualize the network structure and sentiment distribution within communities.

---

## Features
1. **Sentiment Analysis**: Uses Natural Language Processing (NLP) techniques to analyze user emotions (positive, negative, neutral) from social media posts.
2. **Community Detection**: Implements the **Louvain algorithm** for discovering communities within the network based on user interactions and emotional expressions.
3. **Temporal Analysis**: Tracks the evolution of sentiment across time, offering insights into how user emotions fluctuate.
4. **Degree Distribution and Centrality**: Analyzes node importance and connectivity within the network, visualizing key influencers.
5. **Triad Analysis**: Examines the presence of triangular structures in the network to study local group formations.
6. **Emotion-driven Subgraphs**: Creates subgraphs based on user emotions, highlighting the sentiment-specific interactions within the network.

---

## Table of Contents
- [Introduction](#introduction)
- [Problem Statement](#problem-statement)
- [Related Work](#related-work)
- [Proposed System](#proposed-system)
- [Framework](#framework)
- [Analysis and Design](#analysis-and-design)
- [Implementation](#implementation)
- [Results](#results)
- [Conclusion and Future Work](#conclusion-and-future-work)

---

## Introduction
The rise of platforms like X has provided opportunities to explore emotional dynamics in social networks. This project investigates emotional community detection, enabling organizations to understand audience sentiment trends, assess user vulnerability to emotional manipulation, and identify influential groups.

## Problem Statement
The challenge lies in detecting groups of users expressing similar emotions, such as happiness, sadness, anger, or excitement, from a social network. Analyzing user-generated content requires sophisticated techniques that integrate both **sentiment analysis** and **community detection**.

## Related Work
Several methodologies have been explored for community detection and sentiment analysis, including:
- Parallel graph partitioning approaches.
- Adaptive community detection that combines topology and content.
- Emotion ranking and sentiment clustering.

These approaches laid the groundwork for developing a comprehensive emotional community detection model.

---

## Proposed System
The proposed system combines network analysis techniques with sentiment analysis to provide a detailed view of emotional interactions in social media. **Louvain community detection** is applied to group users into communities, followed by a centrality and triad analysis to understand the structure of these communities.

### Key Steps:
1. **Data Preparation**: Load and process social network data.
2. **Sentiment Analysis**: Analyze user sentiment using the `nltk` library.
3. **Community Detection**: Detect sentiment-based communities using the Louvain algorithm.
4. **Temporal Sentiment Analysis**: Visualize sentiment trends over time.
5. **Degree Distribution and Centrality**: Compute and display the network's degree distribution and node importance.
6. **Emotion-driven Subgraphs**: Create subgraphs for positive, negative, and neutral sentiments.

---

## Framework
### Step 1: Prepare the Data
Import necessary libraries (`networkx`, `community`, `nltk`, `matplotlib`) and prepare the dataset.

### Step 2: Perform Sentiment Analysis
Use the `nltk` library to calculate sentiment scores for each user (node), classifying them as positive, negative, or neutral.

### Step 3: Community Detection
Apply **Louvain community detection** to identify user communities based on their sentiment scores.

### Step 4: Temporal Sentiment Analysis
Convert time data to visualize how sentiment evolves over time, recalculating sentiment scores periodically.

### Step 5: Degree Distribution and Centrality
Analyze the overall network structure by calculating degree distributions and identifying key users through **centrality analysis**.

### Step 6: Triad Analysis
Examine triangles in the network to understand local group structures.

### Step 7: Sentiment-driven Subgraphs
Visualize and analyze subgraphs based on sentiment (positive, negative, neutral).

---

## Analysis and Design
The dataset, gathered from social media platforms like Reddit and Twitter, was used to create a network of users where edges represent user interactions. Sentiment analysis was performed to classify user emotions, while community detection helped identify sentiment-driven groups. The design aimed to provide a visual representation of user sentiment, aiding in strategic decision-making for campaigns.

---

## Implementation
The project was implemented using Python, with key libraries like `networkx`, `nltk`, and `matplotlib`. The Louvain algorithm was used for community detection due to its efficiency in handling large networks. Detailed steps for implementation include data processing, network visualization, and sentiment analysis.

---

## Results
The combined use of sentiment analysis and community detection techniques successfully identified emotional communities within the network. These results provide valuable insights into user sentiment dynamics, aiding in public opinion research, targeted marketing, and the prevention of misinformation.

---

## Conclusion and Future Work
By integrating **sentiment analysis** with **community detection**, this project offers a novel approach to understanding user emotions and group dynamics in social media. Future improvements could include:
- Enhancing sentiment analysis accuracy through context-aware models.
- Exploring dynamic community detection to capture real-time changes.
- Expanding the application to other areas like mental health analysis and early intervention strategies.

---

## Sample Code
You can find a sample of the project code [here](./path-to-sample-code).

---

## References
- Girvan, M., & Newman, M. E. J. (2002). Community structure in social and biological networks.
- Hutto, C. J., & Gilbert, E. (2014). VADER: A parsimonious rule-based model for sentiment analysis of social media text.
- Strapparava, C., & Mihalcea, R. (2007). Semeval-2007 task 14: Affective text.
- Blondel, V. D., Guillaume, J. L., Lambiotte, R., & Lefebvre, E. (2008). Fast unfolding of communities in large networks.

---

