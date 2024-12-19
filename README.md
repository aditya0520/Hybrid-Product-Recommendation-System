# Hybrid Product Recommendation System

### Overview
This project is a **Hybrid Product Recommendation System** built to enhance product recommendations by combining **collaborative filtering** and **content-based filtering** techniques, powered by **Singular Value Decomposition (SVD)** and **Natural Language Processing (NLP)** methods.

### Features
- **Collaborative Filtering**: Utilized SVD to capture latent factors in the user-item interaction matrix for personalized recommendations.
- **Content-Based Filtering**: Incorporated product metadata and reviews, analyzed using **TF-IDF** for feature extraction.
- **Sentiment Analysis**: Leveraged **VADER Sentiment Analysis** to refine insights from customer reviews and better align recommendations with user preferences.

### Key Results
- Achieved **77% accuracy** in product recommendations.
- Improved recommendation relevance by integrating sentiment analysis with collaborative and content filtering.

### Dataset
The dataset comprises customer reviews and product information, including:
- **Fields**: Marketplace, Customer ID, Product ID, Product Title, Review Body, Star Ratings, etc.
- **Source**: [Amazon Reviews Dataset](https://www.kaggle.com/snap/amazon-fine-food-reviews).

### Methodology
1. **Data Preprocessing**:
   - Loaded and cleaned data to handle missing or malformed entries.
   - Converted textual reviews into numerical vectors using TF-IDF.
   - Prepared a user-item interaction matrix for collaborative filtering.
   
2. **Collaborative Filtering**:
   - Performed matrix factorization using SVD on the user-item interaction matrix.
   - Reconstructed the matrix to predict missing values and recommend top products.

3. **Content-Based Filtering**:
   - Applied TF-IDF to extract key features from product descriptions and reviews.
   - Matched product attributes with user preferences based on cosine similarity.

4. **Sentiment Integration**:
   - Used VADER to analyze sentiment polarity in review text.
   - Incorporated sentiment scores into the recommendation pipeline for enhanced precision.
