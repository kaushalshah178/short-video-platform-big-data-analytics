# short-video-platform-big-data-analytics

# Introduction
A leading short video company is facing challenges in enhancing its revenue and understanding the users so it wants to take help of Big Data Ecosystem to analyze large amounts of data received from varieties of sources, namely through mobile app and website. This analysis will help them to track the behavior of users so that to customize offers for them to buy paid subscription and also calculate royalties to the video creators do that to make them create more videos, this in turn will enhance their revenues.


# Project Pipeline

<img src="short_video_kaushal_pipeline.png" alt="Project Pipeline" width="1500" height="600">


# Project Goal
The goal the project is to create data pipelines for the short video company which will make the company make appropriate business strategies to enhance their revenue by analyzing users and video data to send offers and royalties to users respectively.


#Data Flow Architecture / Process Flow
1.	A Linux file server receives data files in form of xml and csv periodically after every 2 hours. These two files are coming from the website based on user   interaction methodology.
2.	There is a real time stream following as well from the mobile devices from the mobile app logs in form of json going to kafka topic. 
3.	The file data and stream data is validated, enriched and processed before loading into HDFS. There is a  lookup table in this processing logic as well.
4.	Finally data landed to HDFS needs to be analyzed by some analytical queries.

