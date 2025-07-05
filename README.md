# Enhancing-Customer-Feedback-Analysis-through-NLP
This project develops a scalable, NLP-based automated system to analyze multilingual Amazon customer reviews using BERTopic for topic modeling and BERT for sentiment analysis. The goal is to help businesses extract deeper insights from unstructured feedback, enabling quicker, emotion-aware, and data-driven decisions.

By combining unsupervised topic extraction (BERTopic) and supervised sentiment classification (BERT), the system uncovers both what customers are talking about and how they feel. It was tested on two distinct product categories—Sparkling ICE (a flavored water drink) and Nautica Voyage (a men’s perfume)—demonstrating generalizability across industries.

Key Features-

1. Data Cleaning & Preprocessing: Multilingual Amazon reviews were cleaned, translated, tokenized, and lemmatized.

2. BERTopic for Topic Modeling: Extracted dominant themes without needing predefined topic counts using BERT embeddings, UMAP, and HDBSCAN.

3. BERT for Sentiment Analysis: Classified sentiments (1–5 scale) and grouped them into positive or negative categories using a multilingual BERT model.

4. Sentiment-Keyword Mapping: Linked keywords with sentiment scores to identify what drives satisfaction or dissatisfaction.

5. Visual Analytics: Included bar charts, word clouds, sentiment-over-time trends, and topic distributions for deep interpretability.

6. Evaluation Metrics: Used topic coherence (CV), topic coverage, sentiment distribution, and outlier rates for model validation.

7. Reusable Architecture: Designed as a modular and extensible pipeline suitable for feedback from any domain or platform.

Results Summary-

1. High Topic Coherence: BERTopic produced well-separated, coherent clusters with CV scores above baseline standards.

2. Positive Sentiment Rate: Over 81% of reviews were classified as positive for both products.

3. High Topic Coverage: More than 90% of reviews were captured into meaningful clusters; fewer than 10% were outliers.

Key Insights-

1. Sparkling ICE: Common themes included “flavour,” “taste,” and “health,” with packaging issues noted in negative reviews.

2. Nautica Voyage: Focused on “scent,” “longevity,” and “compliments,” but also revealed concerns about authenticity and lasting power.

3. Sentiment Mismatch Handling: The system successfully identified reviews where polite wording masked negative sentiment—something missed by simpler models.

Tools & Technologies-

1. Languages & Environment: Python, Jupyter Notebook

2. NLP Libraries: spaCy, NLTK, Gensim, TextBlob

3. Topic Modeling: BERTopic (BERT + UMAP + HDBSCAN)

4.  Sentiment Analysis: BERT (bert-base-uncased, multilingual)

5. Evaluation & Visualization: Scikit-Learn, Matplotlib, Seaborn


