Project on AWS.
I have created a automated mailing system using Amazon Web Services such as DynamoDB, AWS Lambda, AWS Event Bridge and AWS SNS.

Some medications which are prescribed by the doctors have a weekly dosage regimen such as VITAMIN D supplements. This can be challenging for patients to follow up. Therefore I created an automation which sends E-mail reminder every week to patients to help them take the supplements on time.

DYNAMODB:
Firstly, i created a table in DynamoDb named PatientReminders with PatientID as partition key.
Then I added the attributes such as Name, Email, StartDate and NotificationTime.
StartDate and NotificationTime are written in UTC timezone and ISO8601 format.
