# TuneMyRun

## Project Idea
Create an application that queues songs for runners based on speed and a track's bpm. Additionally runner's taste in music will also be a factor in the overall selection of the song.

## Tech Stack
S3- For primary data storage  
Airflow - To run on a daily basis to get data from spotify and add to existing database  
*<Scalable, Low latency and high throughput streaming solution. Can compromise on throughput to an extent but not latency*
*Queue and notification system. Maybe SQS and SNS?>*

## Data Source
Million Song Dataset - https://labrosa.ee.columbia.edu/millionsong/
Spotify API - https://developer.spotify.com/documentation/web-api/reference/browse/  
Accelerometer Data Stream - https://www.kaggle.com/vmalyi/run-or-walk

## Engineering Challenge
Ability to handle running streams from lots of users simultaneously and providing near real time song queues from a constantly growing song dataset ~ 300 GB. Also the datasets are from different sources so combining them efficiently will be a challenge.

## Business Value
Music industry is an extremely competitive space and personalization is the key to get ahead of the competition. Applications like tune my run can provide users better running experience

## MVP
Combine using dataset with incoming stream and push to a queue and notification system.

## Stretch Goals
Build a ML algorithm for predicting music taste based on runner's profile
