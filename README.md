# Youtube Data Analytics | End-To-End Data Engineering Project Using AWS

## Introduction
This project demonstrates an end-to-end data engineering pipeline for analyzing YouTube data using AWS services. By leveraging tools like AWS Glue, S3, Lambda, Athena, and QuickSight, the pipeline enables seamless data ingestion, transformation, and visualization. The aim is to provide insights into YouTube video performance, audience engagement, and content trends. This repository serves as a comprehensive guide for building scalable, cloud-native analytics solutions.

## Architecture
![Project_Architecture](Architecture.png)

## Services Used
1. AWS IAM: AWS Identity and Access Management (IAM) enables secure control of access to AWS resources by defining permissions and policies for users, groups, and roles.
2. AWS S3: Amazon Simple Storage Service (S3) is a scalable, durable, and secure object storage service that allows users to store, retrieve, and manage data in the cloud with virtually unlimited capacity.
3. AWS Glue: AWS Glue is a fully managed, serverless ETL (Extract, Transform, Load) service that simplifies data preparation and integration by automating schema discovery, transformations, and job execution across various data sources.
4. AWS Lambda: Lambda is a computing service that allows programmers to run code without creating or managing servers.
5. AWS Athena: Athena is an interactive query service for S3 in which there is no need to load data it stays in S3.
6. QuickSight: Amazon QuickSight is a scalable business intelligence tool that allows you to create interactive dashboards and visualize data from multiple sources in real time.

## Dataset Used
This Kaggle dataset contains statistics (CSV files) on daily popular YouTube videos over the course of many months. There are up to 200 trending videos published every day for many locations. The data for each region is in its own file. The video title, channel title, publication time, tags, views, likes and dislikes, description, and comment count are among the items included in the data. A category_id field, which differs by area, is also included in the JSON file linked to the region.

https://www.kaggle.com/datasets/datasnaek/youtube-new

## Scripts Used
1. [ETL using Lambda function](lambda_function.py)
2. [ETL using AWS Glue](pyspark_code.py)

## Data Visualization
Data visualization was performed using AWS QuickSight.  
[Dashboard](YouTube Data Visualization using Quicksight.pdf)

The following insights were derived.

1. Among all the categories, music videos were the most liked, followed by News and Politics.
2. The dataset lacked clear information about the most-watched channels, but some notable ones included SpaceX and XXXTentacion.
3.   Viewers frequently rewatched music videos.
4.  The majority of the views originated from Great Britain (UK), surpassing those from the USA and California.

## Credits
- This project is based on a tutorial by [Darshil Parmar]([Link to the tutorial](https://github.com/darshilparmar/dataengineering-youtube-analysis-project)).



