# Anomaly-Detection
This project uses different methods for anomaly detection of a timeseries. 

The data used has two variables used in adwords for online marketing: CPC (Cost Per Click) and CPM (Cost Per Thousand). Both of them are a timeseries with matching timestamps and there are three sets of files. One of them has no anomalities while the other two do.

The notebook goes through different ideas in how to tackle this problem:
- Supervized Learning: Since there are no lables, I generated them by clustering the data with DBSCAN. Later, I trained a RandomForest model with them.
- Unsupervized Learning: I built different models in order to see how they perform different. I used KMeans, OneClassSVM, EllipticEnvelope, and IsolationForest.
- ARIMA: Created an ARIMA model that predicts anomlies based on it's residue.

For each approach there is a python widged that visualizes the result for the selected set of files!
