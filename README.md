#  NLP Project | Automated Customer Reviews

Team Members: Hessah · Ghadah · Shatha

Goal: Automatically analyze and summarize product reviews to classify sentiment, cluster product categories, and generate product recommendation summaries using NLP and Generative AI.

# Project Overview
In today’s review-driven market, businesses and customers rely heavily on user-generated content. However, manually analyzing thousands of reviews is inefficient. This project aims to automate the end-to-end process of review analysis using:

Sentiment Classification using Transformer-based models

Product Category Clustering using unsupervised learning and embeddings

Review Summarization using GPT-4 for blog-style recommendation articles

Deployment of a user-friendly web app using Gradio

# Tasks Overview
1. Sentiment Classification
   
Model: distilroberta-base (fine-tuned on balanced_reviews.csv)

Classes: Negative (1–2), Neutral (3), Positive (4–5)

Accuracy: 85.15% | F1 Score: 84.99%

Strength: High performance on positive/negative, neutral still challenging

2. Product Category Clustering
   
Goal: Group products into 4–6 meta-categories

Tech: Sentence embeddings (MiniLM), KMeans, UMAP, t-SNE

Steps: Cleaning → Phrase detection → Embedding → Clustering → Keyword extraction

Libraries: spaCy, sklearn, SentenceTransformers, matplotlib

3. Review Summarization
Tool: GPT-4

Input: Clustered reviews + insights (top-rated, pros/cons, worst product)

Output: Blog-style article per category

Features: Highlights 3 best products + 1 to avoid

# Web App (Gradio)

Tab 1: Sentiment Analysis → Enter a review, get sentiment

Tab 2: Category Summary → Upload CSV, get blog-style summary

CSV Columns Required: name, reviews.text, reviews.rating, categories

## Key Results

Metric	Value
Accuracy	85.15%
Precision	84.77%
Recall	85.15%
F1 Score	84.99%
Tools & Models
Transformers: Hugging Face (distilroberta, MiniLM)

Clustering: KMeans, UMAP, silhouette score

Summarization: OpenAI GPT-4

Deployment: Gradio

# Deliverables

Code + Models

 Gradio App

GPT-4 Blog Summaries

You can see all of our models and datasets and the deployment using this link : https://colab.research.google.com/drive/1-9UKpZsxbQcVCosJ9b3ENvjp6w02CFGw?usp=sharing

PPT Presentation : https://www.canva.com/design/DAGhZW5GLIo/pjljS9XGAcDy0Br2nseMNA/edit?utm_content=DAGhZW5GLIo&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton

PDF Report :https://docs.google.com/document/d/1SCzJjwLbMX3HZm4Aio3Bs-yDWbArnzqhGt2TKwS5Gfs/edit?usp=sharing



