# **Exploring Alexa's ability to discern accents**

## Table of Contents 
1. [Problem](#problem)
2. [Goal](#goal)
3. [Methodology](#method)
4. [Tools](#tools)
5. [Files](#desc)
6. [Architecture](#architect)
7. [Running Our Code](#help)

## Problem <a name="problem"/>
Amazon has been increasing support for accessibility across various accents. However, from our person experience, Amazon’s Alexa appears to sometimes struggle to discerned by Amazon’s Alexa.

## Goal <a name="goal"/>
Our goal is to determine Alexa's ability to recognize different English accents.

## Methodology <a name="method"/>
1. Use AWS Polly to generate speech samples in different accents. 
2. Record some of our own and friend's accents. 
3. Apply AWS Transcribe convert our speech samples into text.
4. Compare how AWS Transcribe did with genereated speech samples and our own. 

## Tools <a name="tools"/>
1. AWS Transcribe - Converting audio meeting recordings into text (https://aws.amazon.com/transcribe/)

2. AWS Polly - Turns text into life like speech (https://aws.amazon.com/polly/)

## File Description <a name="desc"/>
Data - Contains all of our speech samples generated from AWS Polly 

## Architecture <a name="architect"/>
![ArchitectureDiagram](https://github.com/jongmp/Napoli-Polly/blob/main/Diagram.png)


## Running Our Code <a name="help"/>

### Instructions to Ge
1. First, before we generate our speech samples using AWS Polly. We need to first create a S3 bucket that will store all of our speech samples. To do this, log into your AWS Services account. Search for S3 in the search bar at the top. It should bring you to this page. 

![image](https://user-images.githubusercontent.com/48782795/115645085-bacedc80-a2ed-11eb-97d2-723b3a806ed3.png)

We need to then create a bucket where we can store our speech samples. We can do this by selecting the "Create Bucket" button in orange.

![image](https://user-images.githubusercontent.com/48782795/115645277-126d4800-a2ee-11eb-9ed8-71ade1e3f7f5.png)

We need to create a bucket name. We chose our bucket name to be napoli-bucket and we allowed public access for this bucket. Afterwards, we can select Create Bucket at the bottom of the page. Now, we are ready to generate our speech samples and upload them to the S3 bucket.

2. Next, we generated our speech samples using AWS Polly. (https://aws.amazon.com/polly/) After logging into your AWS Services account, you should be able to enter text that can be read in different languages and voices. We did the following for Spanish, French, and Hindi for a variety of different texts. All the mp3 files were uploaded to the s3 bucket using the graphical user interface (synthesize to S3). 

![image](https://user-images.githubusercontent.com/48782795/115628044-fc4f8f80-a2cd-11eb-8243-41a59f7a1353.png)

![image](https://user-images.githubusercontent.com/48782795/115641780-c4554600-a2e7-11eb-9553-046fb15cf73a.png)

After selecting the "Synthesize to S3" Button, a pop up window will be created. 

Our audio files can be downloaded through our [MP3 files](https://github.com/jongmp/Napoli-Polly/tree/main/MP3%20files) folder on this GitHub Repo. 



2. Next, through SageMaker, we utilized AWS Transcribe. 


4. Extract names 
5. Put names into dataframe 
6. for each mps file, we createed a link and a job name 
