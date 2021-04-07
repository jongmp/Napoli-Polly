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

## To Run Our Code <a name="help"/>
description on how to run our code 
possibly include gifs to demo
include audio files samples
