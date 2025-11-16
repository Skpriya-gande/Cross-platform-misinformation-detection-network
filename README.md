##🛰️ Cross-Platform Misinformation Detection Network

A unified machine learning and graph-based architecture designed to detect misinformation across multiple online platforms using text semantics, propagation behavior, and graph learning.

📌 Project Overview

This project focuses on building a Cross-Platform Misinformation Detection Network capable of identifying misleading content across diverse online platforms. Unlike single-dataset models, this system uses three heterogeneous misinformation datasets, ensuring high generalization and robustness.

Our core contribution is the proposed CTPP-GNN (Cross-Platform Text & Propagation Pattern Graph Neural Network), designed to jointly analyze text content and its propagation patterns on social platforms.

📂 Datasets Used

To ensure cross-domain learning, the system is trained/evaluated on three diverse datasets:

Fake News / News Articles Dataset – long articles labeled as real or fake.

Twitter Misinformation Dataset – short-form social content including rumors and verified posts.

LIAR / PolitiFact Dataset – claim-level truthfulness data verified by experts.

This multi-dataset approach significantly improves cross-platform performance.

🏛️ Existing Models (Baselines)

To benchmark performance, the following established misinformation detection models were implemented:

1️⃣ BiLSTM (Bidirectional LSTM)

Captures sequential patterns and context from text in both directions.

2️⃣ GCN (Graph Convolutional Network)

Builds static graph structures to model relationships between posts, users, or shared content.

3️⃣ Multimodal Transformer

Processes multiple features such as text, metadata, and user information using transformer attention.

4️⃣ TGN (Temporal Graph Network)

Models dynamic propagation graphs and learns time-aware misinformation patterns.

These baselines allow clear comparison with the proposed CTPP-GNN model.

🚀 Proposed Model: CTPP-GNN
Cross-Platform Text & Propagation Pattern Graph Neural Network

The proposed architecture integrates textual embeddings, propagation structures, and cross-dataset fusion using a graph-based deep learning pipeline.

Key Components

✔ Text Encoder
Uses transformer-based embeddings (e.g., BERT/DistilBERT) for semantic understanding.

✔ Propagation Graph Builder
Constructs social interaction graphs using:

retweets / shares

replies / comments

user–post relationships

temporal propagation signals

✔ Graph Neural Network Core
GNN layers learn structural misinformation patterns at the graph level.

✔ Cross-Platform Fusion Layer
Combines representations from all datasets in a unified embedding space.

✔ Classification Layer
Predicts whether input content is misinformation or genuine.

🌐 Deployment

The complete project has been successfully deployed as a live website, allowing users to:

✔ Enter text or upload content for misinformation detection
✔ View prediction results in real time
✔ Interact with a user-friendly interface built on top of the trained CTPP-GNN model
✔ Access a fully functional backend pipeline that performs preprocessing, inference, and classification

This deployment demonstrates the real-world applicability and usability of the system.

🔬 Work Completed

✔ Preprocessing and unification of 3 misinformation datasets
✔ Implementation of baseline models: BiLSTM, GCN, Multimodal Transformer, TGN
✔ Design and training of the proposed CTPP-GNN architecture
✔ Cross-platform evaluation and performance comparison
✔ Development of REST API for inference
✔ Deployment of the model as a web application
✔ Complete documentation of the workflow

📊 Summary of Results

CTPP-GNN achieved the best performance among all baselines.

Graph-based propagation modeling significantly improved detection accuracy.

Cross-dataset training enhanced generalization to unseen platforms.

The deployed website showcases real-time misinformation classification capability.
