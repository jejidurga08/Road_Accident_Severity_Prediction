📌 Overview
This project leverages Graph Neural Networks (GNNs) and Transformer-based models to predict road accident severity using real-world traffic crash data. By structuring road networks as graphs, the system captures spatial relationships between accident locations, road features, and environmental factors to enhance prediction accuracy.

📂 Dataset & Features
We use accident datasets from Los Angeles (CA) and other regions, converted into a graph structure using PyTorch Geometric. The dataset includes:

Node Features: Accident locations, road attributes, time of crash.

Edge Features: Road connectivity, traffic conditions, direction, and angular features.

Severity Labels: Categorized from 0 (no accident) to 7 (most severe).

🔍 Machine Learning & Deep Learning Models
We compare traditional machine learning with advanced deep learning for severity prediction:

✅ Machine Learning Baseline
XGBoost (XGBClassifier): A tree-based gradient boosting model used for comparison.

🚀 Deep Learning Approaches
Graph Convolutional Network (GCN): Captures spatial dependencies in road networks.

GraphSAGE: Efficient learning using neighborhood sampling.

Graph Transformer: Uses self-attention for long-range dependencies.

TRAVELNet: Integrates spatial & temporal accident patterns.

TRAVEL Angular Model: Incorporates angular information to improve risk assessment.

📊 Performance Metrics
To evaluate model effectiveness, we use:
✔ Accuracy - Correctly classified severity levels.
✔ F1 Score - Balances precision & recall.
✔ Precision & Recall - Measures model reliability.
✔ MCC (Matthews Correlation Coefficient) - Robust evaluation for imbalanced datasets.
✔ Jaccard Index - Measures similarity between actual & predicted severity.
✔ Execution Time - Computational efficiency of each model.

🎨 Visualization
Using Matplotlib and NetworkX, we visualize:

Accident location graphs (nodes = accident sites, edges = road connections).

Severity level distribution (actual vs predicted values).

🌍 Web App Deployment (Flask & Streamlit)
A Flask-based web application allows users to input accident-related details (driver age, weather, road type, etc.) and receive real-time severity predictions.

🌐 App Features
✅ Simple user interface for inputting accident details.
✅ Feature encoding for categorical variables (e.g., road type, accident cause).
✅ Pretrained model loading for fast predictions.
✅ Dynamic result display with severity levels & key risk factors.

🏆 Results & Findings
Transformer-based models outperform traditional machine learning in severity prediction.

TRAVEL Angular Model achieves the highest accuracy (88.72%) and F1-score (85.58%).

Graph-based learning significantly improves accident risk assessment.
