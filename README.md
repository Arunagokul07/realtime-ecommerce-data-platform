# Real-Time E-Commerce Event Processing & Data Reliability Platform

## About The Project

I am building this project to understand how real time data engineering works in real-world e-commerce environment. 

In an e-commerce application, customers continuously perform different activities such as viewing products, adding products to their cart and placing orders. all these activities generate data continuously. My goal is to built a data pipeline that can collect all these events, process them in a near real time and make the data reliable enough for analysis.

I also want to understand how the data engineer handles the problems that can happen in real-world data instead of working only with clean datasets.

## Business Problem

An e-commerce company can receive a large number of events from it's website or mobile application every second.
For example :

  - A customer views a product
  - The customer clicks on the product
  - The customer adds it to the cart
  - The customer places an order

if these events are not processed properly. the company may get incorrect information about the sales and customer activity.

Some of the problems that can happen are: 

  - The same event may arrive more than once
  - Some records may have missing values
  - Incorrect values may arrive later than expected
  - the number of events may suddenly increase

Because of these problems, business teams may not get accurate or timely informations.

## What I Want To Built

I want to built a pipeline that can :

1. Generate E-commerce events using python.
2. Send this events continuously to a streaming system.
3. Process the events in near real time.
4. Check whether the incoming data is valid.
5. Identify duplicate events.
6. handle events that arrive late.
7. Calculate useful business metrics.
8. Store the processed data for further analysis.

## Problems I Want To Handle

## 1. Duplicate Events
   Sometimes the same event may be received more than once.
For example:

Event E1001 - Purchase
Event E1001 - Purchase

The pipeline should identify this as duplicate and make sure this purchase is not continued twice.

## 2. Invalid Data 
    The incoming data may contain incorrect or missing values.
For Example:

Customer_id = NULL
Quantity = -2
Price = NULL

I want the pipeline to identify these records instead of allowing them to affect the final analysis.

## 3. Late Events

    An event may happen at 10.05 AM but reach the processing system at 10.08 AM. 
I want to understand how real time data pipelines deal with these delayed events.

## 4. Sudden Increase In Events*
    Normally the system may receive around 100 events per minute but during the sale, it could suddenly receive thousands of events. 
I want to test how the pipeline behaves when the event volume increases.

## Business Questions

After Processing the data, I want the system to answer questions such as:

- How many orders where placed in last 5 minutes?
- How much revenue was generated?
- Which products are getting the most views?
- Which products are generating the most sales?
- How many unique customers are active?
- How many duplicate events were recieved?
- How many invalid events were rejected?
- Did the event volume suddenly increase or decrease?

## Initial Scope

  For the first version i will focus on :
    - Customer events
    - Product events
    - cart events
    - Purchase events
    - Real-time event ingestion
    - Data validation
    - Duplicate detection
    - Real-time agrregation
    - Sorting processed data
    - SQL- based analysis

  I will add more features once the desired pipeline is working.

 ## Expected Outcome :

    By Completing this project, I want to understand How the real world streaming data pipeline is designed and implemented. 
The final pipeline should be able to take continuously generated E-commerce events, process them, identify problematic data and produce reliable information that can be used for analysis.

I will also document the problem I face while building the project and how i solve them.
  
    
    

