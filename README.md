#  AWS Automated Medication Reminder System  

##  Project Overview  
This project implements a serverless, event-driven email notification system on **Amazon Web Services (AWS)** to help patients adhere to their weekly medication regimen.  

Certain medications, such as **Vitamin D supplements**, follow a weekly dosage schedule, which can be challenging for patients to remember. This system automates email reminders to ensure timely medication intake.  

By leveraging **AWS**, the solution ensures improved adherence and patient outcomes without the need for manual intervention.  

---

##  Tech Stack & AWS Services  

- **Amazon DynamoDB** – NoSQL database for storing patient and medication details.  
- **AWS Lambda** – Serverless function that processes reminders and triggers notifications.  
- **Amazon SNS** – Manages and sends email notifications to patients.  
- **AWS EventBridge** – Schedules and triggers AWS Lambda functions on a weekly basis.  

---

##  System Architecture & Workflow

**Data Storage (Amazon DynamoDB)**  
- Stores patient details, medication name, dosage frequency, and email addresses.
     
**Automation & Scheduling (AWS EventBridge)**  
- Triggers the AWS Lambda function at scheduled intervals (weekly).
   
**Logic & Processing (AWS Lambda)**  
- Fetches patient data from DynamoDB.  
- Formats and prepares email reminders.  
- Publishes messages to Amazon SNS for email delivery.     

**Email Notification (Amazon SNS)**  
- Delivers email reminders to patients based on their stored medication schedules.  

---

This project is completely serverless!
 
