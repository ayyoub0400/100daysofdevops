# Day 1 - CloudWatch Metrics

Task:
1. Create a CloudWatch Alarm that sends an email notification when the CPU usage of an EC2 instance exceeds a threshold.
2. Create a Status Check Alarm that sends an email notification when the status of an EC2 instance changes to "stopped".

Solution:
1. Via AWS Console
2. Terraform

# Notes

What is CloudWatch?

AWS CloudWatch is a monitoring service that monitors your AWS resources and applications. It provides metrics, logs, and alarms that you can use to monitor and manage your resources.

Default EC2 instance metrics:
- CPU usage
- Network traffic
- Disk usage

Status Checks:

System Status Checks - These monitor the status of the AWS system where the EC2 runs. Examples of problems that can cause a system status check to fail include:

- Network connectivity issues
- Loss of system power
- Software/Hardware failures on the host

Instance status checks - Monitor the software and network configuration of the EC2 instance. Examples of problems that can cause an instance status check to fail include:

- Incorrect network configuration
- Corrupted filesystem
- Exhausted Memory

Miscellaneous:

- RAM utilisation is a custom metric and is not a default metric.
- Default EC2 monitoring interval is 5 minutes however detailed monitoring can be configured to probe every minute at an extra cost
- CloudWatch can be used on-prem via installing the AWS SSM & the CloudWatch Agent.
