# Dynamodb Provision capacity scaling by schedule
This project shows how to change provision capacity of DynamoDB table based on a schedule. This is helpful in certain use cases when you need instant additional capacity at a certain time point of day/week.

The Cloudformation template demonstrates adjusting Write capacity on the schedule but a similar approach can be followed for Read capacity.

Some of the parameters of cloudformation template that need to updated :
1. RoleArn - Role that can perform autoscaling of the DynamoDB capacity
2. PeakCronSchedule/OffPeakScheduleCron : Cron expression for your schedule
3. Low and high Write capacity

