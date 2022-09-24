# case study
https://github.com/implydata/candidate-exercises-public/tree/master/Customer%20Success/SA/DataEngineeringProject/Applicant#part-b-case-study

Server: 2x 8-core HT processors (16 cores total, 32 hardware threads) 64GB memory 600GB SSD disk


In this exercise we will provide you with a set of customer requirements for Koala Maximization, Ltd. ("Koala" for short), the company that operates the popular web property http://koalastothemax.com/. Your goal will be to suggest how they can deploy Imply to best meet their needs.

Customer requirements
Koala has a dataset composed of visits to their web site, annotated with session ID, path visited, and attributes about the visitor like "city" and "browser". They want to build dashboards based on this dataset as well as be able to explore this dataset interactively.
An example data point for a single hit is below:

How many unique sessions were there last month?
How many unique sessions are there per day in each country?
Koala has one type of hardware available in its datacenter, with the following specs:


Your challenge is to write a recommendation for Koala hitting the following points:
How many servers will be necessary for an analytics cluster for one year of this dataset
How these servers should be configured (JVM config, Druid runtime.properties)
 How Imply can be used to answer the two sample queries provided by Koala (number of unique sessions in a particular month; number of unique sessions per country in a particular day).
Some aspects of your recommendation will need to be based on guesswork. This is totally normal, even for a real customer engagement! Whenever you are guessing, please point out what assumptions you made, and what additional information you would need in order to refine your guess.


Like the coding challenge, it is much more important to have a reasonable recommendation for each point that to have the best possible recommendation. We are not looking for perfection. Rather, we are looking for a good starting point that could be improved with more research.
Please include some details about how you arrived at the conclusions in your recommendation. This is even more important to us than the actual recommendations.
Suggested resources
You may find these resources helpful when putting together your recommendation:
Imply documentation:





[Data Section]
 sample data type: json 
 each message size: 611 bytes
 daily hits: 200 mil
 wants to keep a year data:

 1. Daily ingest
=> 611 * 200,000,000 => 122,00200,000,000 (bytes)
 -> 113.807619 GB per day
 
2. Ingesting in a given time
 -> 

[Query Section]
