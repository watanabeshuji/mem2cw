# Overview
mem2cw is CloudFormation template for Lambda function 
that Memory Usage as CloudWatch Metric Data using CloudWatchLogs subscription filter.

# Usage
Login to AWS management console and create CloudFormation stack with logs2sns.yml(logs2sns2.yml).
See: http://dev.classmethod.jp/cloud/aws/send-lambda-memory-usage-to-cloudwatch/ 

# CloudFormation Parameters
- Namespace: Namespace for CloudWatch Metric

# How it works?
- Create IAM Role for Lambda function.
- Create Lambda function process CloudWatch Logs streaming event (filter and put CloudWatch Metric).
- Add permission to Lambda function to invoke from CloudWatch Logs

# Licence
- The MIT License (MIT)
