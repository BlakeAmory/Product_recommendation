# SkinCare Recommender

This project is a content-based recommendation engine that recommends scraped Dermstore skincare products based on product ingredients and descriptions 🫧

## Architecture

1) Skincare product data (Moisturizers, Treatments/Serums, Cleansurs/Exfoliators) scraped from [Dermstore](https://dermstore.com) using **Scrapy**
2) Ingredients standardized with [Skincarisma's Ingredient Analyzer Tool](https://skincarisma.com) using **Selenium Webriver**
3) Product ingredient and description texts vectorized using **BERT embeddings** and **TruncatedSVD/TSNE**
4) Products recommended based on highest **Cosine Similarity**

## Installation

Clone the github repository

```bash
git clone https://github.com/BlakeAmory/Product_recommendation.git
cd Product_recommendation
```

Install the dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
streamlit run app/app.py
```

## ✨ Results ✨

The results of running the app are shown below:

![final_skincare.gif](final_skincare.gif)
