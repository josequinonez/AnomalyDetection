# AnomalyDetection
Techniques to detect outliers using unsupervised anomaly detection and detect anomalies in test data using Semi-supervised anomaly detections

The goal of this notebook is to show some strategies to find outliers in a dataset.
- In **Unsupervised anomaly detection** we know that a few outliers are included in the dataset. We may use two approaches:
    - Unsupervised outlier detector algorithms: Identify a high density cloud of data points close to each other and have them marked as normal (inliers), and assume that those data points outside of this cloud are outliers.
    - Clustering analysis: Assume that there are two custers of data: one that groups normal data, and the other cluster groups the outliers.
- In **Semi-supervised anomaly detection** we know that outliers are not included in the dataset, so we only have normal data for training. It learns the common characteristics of normal data and sets a threshold of what a normal data item should be. Test points are then measured to asses their closeness to this threshold. There are two approaches:
    - Using different metrics to measure distance from each test point to the normal data centroid to see if it exceeds the threshold.
    - Using a Neural Network Autoencoder error loss as a threshold distance to assess normality.

Jose Quinonez
