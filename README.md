
# Cat Bathroom Monitoring System
## Introduction
### What is the purpose of the cat bathroom monitoring system?
This project aims to improve the health and well-being of our family cat, Atticus by monitoring his bathroom behavior with a fully automated system. The idea of this project was formed when Atticus was diagnosed with urinary traction disease in 2019 and our vet suggested that we keep track of his bathroom habits.

To accomplish this, I developed a software program that utilizes the image recognition technology provided by the [jetson-inference library](https://github.com/dusty-nv/jetson-inference). This works in conjunction with a camera installed in front of Atticus' litterbox. Every time Atticus uses the litterbox, the system records his entry and departure times. The data is then automatically processed and sent to a Postgres database through an efficient **ETL pipeline**. A data visualization service has also been set up using Metabase to help us analyze the data, and we can view graphs of Atticus' bathroom behavior through a user-friendly web app.

*Note: This system is made, assuming that one litterbox is used by one cat.* 

## What did I do to develop this system?
### ***Local setup (Version 1)***

### Step 1: Develop a computer vision software application 
This software application automatically records the timestamps corresponding to each instance of a cat using the litterbox.
#### Refer to [its Github repo](https://github.com/emma-jinger/CatWatcher) for more details.
### Step 2: Set up a data pipeline
The data pipeline watches new data and load it to a database. Design and implement a data pipeline that continuously monitors for incoming data and efficiently loads them into a designated database for further processing and analysis.
#### Refer to [its Github repo](https://github.com/emma-jinger/cat_data) for more details.

### Step 3: Build a web app that will present the data
#### Refer to [its Github repo](https://github.com/emma-jinger/cat_bathroom_monitoring_system_web_app) for more details.

### ***Using Docker (Version 2)***
## What skills did I demonstrate in making this system? 
To be continued...
