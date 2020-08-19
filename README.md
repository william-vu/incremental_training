# Keeping your ML model in shape with Kafka, Airflow and MLFlow
### How to incrementally update your ML model in an automated way as new training data becomes available
This repo is forked from [here](https://github.com/MBKraus/incremental_training). 
It shows how to use  [Kafka](https://github.com/apache/kafka), [Airflow](https://github.com/apache/airflow), and [MLFlow](https://github.com/mlflow/mlflow) to update a deployed model. 

The orignial medium post is [here](https://medium.com/vantageai/keeping-your-ml-model-in-shape-with-kafka-airflow-and-mlflow-143d20024ba6) 

It simulates the (new) incoming data  by replaying/writing (MNIST) images to a predefined Kafka topic. One consumer reads data from this topic and uses this data to update model. 
