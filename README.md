# 10_InternetUsuageClustering_202401100300040
This project analyzes internet users by clustering based on browsing behavior, then classifying them if user types are known. It uses metrics like device usage and site visits to uncover patterns and predict user categories, aiding in personalization and platform optimization.
Internet Usage Clustering & Classification
This project focuses on analyzing and grouping internet users based on their device usage time, site categories visited, and visit frequency. The goal is to uncover patterns and classify users into distinct behavioral segments.

# Features
Unsupervised Learning: Grouping users using KMeans clustering.

Supervised Learning: Predicting user types using a Random Forest Classifier.

Evaluation Metrics: Includes accuracy, precision, recall, and F1-score.

Visualizations: Confusion matrix heatmap and cluster scatter plots.

# Dataset Structure
Ensure your dataset (data.csv) has the following columns:


Column Name	Description
Device_Usage_Time	Time spent on device (e.g., in hours)
Visit_Frequency	Number of site visits
Social_Media	Engagement with social media platforms
Shopping	Engagement with shopping websites
User_Type (optional)	Label for classification (0/1/2)
You can modify or simulate the dataset for experimentation.

# Results
🔹 KMeans Clustering (Unsupervised Learning)
The KMeans algorithm was used to group users into three behavioral clusters based on their internet usage features. Here’s the distribution:
---

# **Results: KMeans Clustering (Unsupervised Learning)**

The KMeans clustering algorithm was applied to group users into **three behavioral clusters** based on their internet usage features. Below is the distribution of users across the three clusters:

# Cluster Distribution:
```
Cluster 0: 45 users — Likely low-usage users  
Cluster 1: 38 users — Possibly social media-focused users  
Cluster 2: 17 users — Possibly heavy or shopping-oriented users
```

# Cluster Characteristics**:
- **Cluster 0**: Users with lower device usage and visit frequency, potentially casual or infrequent internet users.
- **Cluster 1**: Users exhibiting higher social media engagement, suggesting they are more active in social networks.
- **Cluster 2**: Users who exhibit significant interaction with shopping sites, possibly high-frequency shoppers.


📝 Insights:

The model performs best on Class 2.

Precision and recall are low for Class 1, suggesting room for improvement.

Additional data, feature selection, or model tuning could improve results.

# Visualizations
✅ Cluster Plot: Visualizes how users are grouped in feature space (usage vs. frequency).

✅ Confusion Matrix Heatmap: Shows the classification performance across user types.

# Setup
To set up and run this project:

Clone the repository to your local machine.

Install the necessary libraries using pip:

bash
Copy
Edit
pip install pandas numpy matplotlib scikit-learn
Place your dataset (data.csv) in the project directory or modify the code to point to your dataset location.

Run the Python script to execute the clustering and classification algorithms.

# Credits & References
Libraries: pandas, numpy, matplotlib, scikit-learn

Project Guide: DTU course on Data Science Applications

Inspiration: Real-world user segmentation for personalization
