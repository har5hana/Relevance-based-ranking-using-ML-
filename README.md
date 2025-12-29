# Relevance-based-ranking-using-ML-
Built an interpretable Relevance based ranking using ML . Used TF-IDF and structural features, trained a pairwise ranker, and evaluated with NDCG to model relative relevance between documents.

Overview

This project implements a Learning-to-Rank (LTR) system to rank cultural, lifestyle, and knowledge-based articles. Unlike typical black-box ML projects, this emphasizes interpretable features, pairwise ranking, and proper evaluation using ranking metrics.

Problem Statement

Given a user query, the goal is to rank documents by relevance, ensuring the most useful content appears first. Relevance is modeled on a graded scale (0–3), simulating real-world search behavior.

Approach

Feature Engineering

TF-IDF similarity between query and document

Query length

Document length

Pairwise Learning-to-Rank

Generated document pairs based on relevance

Trained a Logistic Regression model to predict relative ordering

Evaluation

NDCG@3 used to measure ranking quality

Ablation studies show feature contribution

Results
Model	NDCG@3
TF-IDF Only	0.xx
Full Model	0.yy

Adding structural features improved ranking performance.

Pairwise training ensures relative relevance is correctly modeled.

Tech Stack

Python, Pandas, NumPy, Scikit-learn, Jupyter Notebook

Future Work

Incorporate BM25 scoring

Experiment with LambdaRank or XGBoost Ranker

Expand dataset for more diverse queries

Author

Harshana Yadav
