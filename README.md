# NBA-Notification-System
## Description:
THis is a system that sends an alert via sms or text(according to preference) to a user over the NBA game stats using Amazon SNS.
It implements the use of the following: AWS Lambda, AWS Simple Notification Service, Amazon EventBridge and Amazon IAM 

## Prerequisites:
1. A functional AWS account
2. An API key from sportsdata.io(IT'S FREE!)
   
## Structure
![Proj structure](https://github.com/mbengiivy/NBA-Notification-System/blob/main/30a80021-58d5-4177-bcd1-0530f4246a1a.jpg)

## Worflow
The set time for the eventbridge rule sends a trigger to the lambda function.

The lambda function sends a request to the sportsdata api

The data is sent back to the function

The data is sent to the subscribed users via SNS

The task is to set up the system to send notifications on the game stats. I took the challenge to upgrade my code to not only send game notifications but also send stadiums available as well. 
I also got the chance to learn the AWS services more and interact with different settings eg. roles and policies. 
