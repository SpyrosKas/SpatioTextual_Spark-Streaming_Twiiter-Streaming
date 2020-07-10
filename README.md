# SpatioTextual_Spark-Streaming_Twitter-Streaming
Processing Real-Time Twitter streaming data and executing Spatio-Textual queries, using Spark Streaming.

[![Contributors][contributors-shield]][contributors-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- GETTING STARTED -->
## Getting Started


### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* tweepy
```sh
pip install tweepy
```
* [Spark Streaming](https://spark.apache.org/docs/latest/streaming-programming-guide.html)

### Installation

1. Create a new twitter app and get your credentials at [https://developer.twitter.com/en](https://developer.twitter.com/en)
2. Clone the repo
```sh
git clone https://github.com/SpyrosKas/SpatioTextual_Spark-Streaming_Twitter-Streaming.git
```
3. Install tweepy 
```sh
pip install tweepy
```
4. Enter your credentials in `receive-Tweets_coordinates.py`
```python
consumer_key    = 'ENTER YOUR CONSUMER_KEY'
consumer_secret = 'ENTER YOUR CONSUMER_SECRET'
access_token    = 'ENTER YOUR ACCESS_TOKEN'
access_secret   = 'ENTER YOUR ACCESS_SECRET'
```
<!-- USAGE EXAMPLES -->
## Usage
1. Run `receive-Tweets_coordinates.py`
```sh
python3 receive-Tweets_coordinates.py
```
2. Run `Spark_Stream_App.ipynb` until line:
```python
ssc.start()
```
3. Wait for the first two batches(20s) and run the visualization code block.
4. To stop SparkContext
```python
ssc.stop()
```
5. Stop socket
```sh
^C
```






<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/SpyrosKas/SpatioTextual_Spark-Streaming_Twitter-Streaming.svg?style=flat-square
[contributors-url]: https://github.com/SpyrosKas/SpatioTextual_Spark-Streaming_Twitter-Streaming/graphs/contributors
[stars-shield]: https://img.shields.io/github/stars/SpyrosKas/SpatioTextual_Spark-Streaming_Twitter-Streaming.svg?style=flat-square
[stars-url]: https://github.com/SpyrosKas/SpatioTextual_Spark-Streaming_Twitter-Streaming/stargazers
[issues-shield]: https://img.shields.io/github/issues/SpyrosKas/SpatioTextual_Spark-Streaming_Twitter-Streaming.svg?style=flat-square
[issues-url]: https://github.com/SpyrosKas/SpatioTextual_Spark-Streaming_Twitter-Streaming/issues
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555
[linkedin-url]: https://gr.linkedin.com/in/spyros-kasdaglis
