# PMGSY Project Scheme Classifier

## Overview

This project develops a machine learning model using IBM Cloud Lite's AutoAI to automatically classify rural road and bridge construction projects under the Pradhan Mantri Gram Sadak Yojana (PMGSY) into their correct scheme categories. By leveraging physical and financial project attributes, the model supports government bodies and policymakers in efficient project monitoring, transparent budget allocation, and impact assessment, enabling better decision-making for rural infrastructure development.

## Features

- Automated multiclass classification of PMGSY projects by scheme using project data.
- Utilizes IBM AutoAI for pipeline building—including feature engineering, hyperparameter tuning, and model optimization.
- High accuracy achieved (92.4%) using a Batched Tree Ensemble (XGB Classifier).
- Deployment as an online service on IBM Cloud, enabling real-time project classification.
- Provides prediction probabilities alongside class labels for transparency.

## Dataset

- Source: [AI Kosh PMGSY Dataset](https://aikosh.indiaai.gov.in/home/datasets/details/pradhan_mantri_gram_sadak_yojna_pmgsy.html)
- Contains physical and financial details of rural road and bridge projects across various Indian states.

## Technology Stack

- IBM Watson Studio AutoAI and watsonx.ai Runtime
- Python for scripting and API testing
- IBM Cloud Lite for model deployment
- Relevant Python libraries: scikit-learn, xgboost, lightgbm, snapml, lale

## How It Works

1. Data is input including features like number of roads and bridges sanctioned, length of sanctioned roads, cost, location, etc.
2. AutoAI automates data preprocessing, model selection, and training, generating multiple pipelines.
3. The best-performing pipeline is selected based on accuracy and other evaluation metrics.
4. The model is deployed as an API on IBM Cloud for real-time predictions.
5. New project inputs are fed to the deployed service to obtain scheme classification with confidence scores.

## Results

- The selected model achieved 92.4% accuracy on holdout validation data.
- The classifier predicts among multiple schemes such as PMGSY-I, PMGSY-II, RCPLWEA, and others.
- Predictions come with confidence scores to assess certainty.

## Future Enhancements

- Integrate real-time project updates and additional data sources (e.g., satellite imagery).
- Explore advanced algorithms including deep learning models.
- Develop comprehensive dashboards for geographic and temporal analysis.
- Extend to other government infrastructure schemes.

## References

- [AI Kosh PMGSY Dataset](https://aikosh.indiaai.gov.in/home/datasets/details/pradhan_mantri_gram_sadak_yojna_pmgsy.html)
- [IBM AutoAI Documentation](https://www.ibm.com/docs/en/watsonx/w-and-w/2.0.0?topic=models-autoai)
- [IBM watsonx.ai API Documentation](https://cloud.ibm.com/apidocs/watsonx-ai)
