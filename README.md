# Mood-Based Movie Recommendation System

## Overview
This project focuses on building and evaluating intent-aware and mood-based movie recommendation system models to address common challenges faced by modern streaming platforms. Traditional recommender systems rely heavily on historical user behavior and popularity metrics, which often results in decision fatigue, limited personalization, and poor alignment with a user’s immediate emotional or contextual needs. This project explores alternative recommendation strategies that integrate natural language processing (NLP), semantic similarity, and emotion-aware filtering to improve recommendation relevance and user satisfaction.

## Problem Statement
Movie streaming platforms face several key issues:
- Paradox of Choice: Extremely large content libraries overwhelm users and cause decision fatigue
- Static Recommendations: User-based and item-based filtering methods fail to capture real-time intent or mood
- Context and Availability Gaps: Recommendations lack situational awareness and emotional alignment

## Dataset
-Link: https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset
- Size: 45,000+ movies
- Key Features:
  - title
  - genres (JSON format)
  - overview (raw text)
  - vote_average
  - vote_count

## Recommendation Models

### 1. Popularity-Based Model
- Uses weighted ratings derived from vote_average and vote_count
- Best suited for generic discovery queries such as “What’s popular?”
- Strength: Safe, high-quality recommendations
- Limitation: Impersonal

### 2. Content-Based Model (TF-IDF)
- Applies TF-IDF vectorization to movie overviews
- Uses cosine similarity to recommend movies with similar plots
- Strength: Effective for “more like this” queries
- Limitation: Keyword dependency

### 3. Mood-Based Hybrid Model
- Uses emotion classification (GoEmotions) on movie overviews and genres
- Filters and ranks movies based on detected user mood
- Strength: Emotionally aligned recommendations
- Limitation: Requires explicit mood input

### 4. Context-Aware Semantic Model
- Applies semantic embeddings and cosine similarity
- Designed to handle complex, intent-driven natural language input
- Strength: Captures nuanced contextual meaning
- Limitation: Higher computational cost

## Evaluation Metrics
- Relevance
- Diversity
- User Satisfaction (qualitative)

## Tools & Technologies
- Python
- Google Colab
- Natural Language Processing (TF-IDF, cosine similarity)
- Emotion Classification (GoEmotions)

## Future Work
- UI/UX development
- Additional parameters (e.g., runtime, release year)
- User history integration
- Real-time feedback loop using reinforcement learning
- Integration of Large Language Models (LLMs)

