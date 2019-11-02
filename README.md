Build a product recommendation engine


This notebook contains steps and code to create a recommendation engine based on shopping history, deploy that model to Watson Machine Learning, and create an app with PixieApps. This notebook runs on Python 3.x with Apache Spark 2.1.

Table of contents :
Setup
Load and explore data
Create a KMeans model
Prepare data
Create clusters and define the model
Persist the model
Deploy the model to the cloud
Create deployment for the model
Test model deployment
Create product recommendations
Test product recommendations model

We'll be using a few libraries for this exercise:

Watson Machine Learning Client: Client library to work with the Watson Machine Learning service on IBM Cloud. Library available on pypi. Service available on IBM Cloud.
Pixiedust: Python Helper library for Jupyter Notebooks. Available on pypi.
ibmos2spark: Facilitates Data I/O between Spark and IBM Object Storage services

i will use the k-means implementation to associate every customer to a cluster based on their shopping history.
and will Create 100 clusters with a k-means model based on the number of times a specific customer purchased a product.

in last : i Create an online deployment for the model
