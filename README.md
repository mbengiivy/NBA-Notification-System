# NBA-Notification-System
## Description:
THis is a system that sends an alert via sms or text(according to preference) to a user over the NBA game stats using Amazon SNS.
It implements the use of the following: AWS Lambda, AWS Simple Notification Service, Amazon EventBridge and Amazon IAM 

## Prerequisites:
1. A functional AWS account
2. An API key from sportsdata.io(IT'S FREE!)
   
## Structure
![Proj structure](https://github.com/mbengiivy/NBA-Notification-System/blob/main/WhatsApp%20Image%202025-01-23%20at%2013.25.23.jpeg)

## Worflow
1. The set time for the eventbridge rule sends a trigger to the lambda function.
2. The lambda function sends a request to the sportsdata api
3. The data is sent back to the function
4. The data is sent to the subscribed users via SNS

The task is to set up the system to send notifications on the game stats. I took the challenge to upgrade my code to not only send game notifications but also send stadiums available as well. 
I also got the chance to learn the AWS services more and interact with different settings eg. roles and policies. 

NB. You must set the environment variables(NBA_API_KEY and SNS_TOPIC_ARN)in the configurations bar in lambda
