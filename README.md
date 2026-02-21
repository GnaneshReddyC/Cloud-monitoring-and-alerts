company: CODTECH IT SOLUTION

NAME:GNANESH REDDY C

INTER ID:CTIS5317

DOMAIN: CLOUD COMPUTING

DURATION: 4 WEEKS

MENTOR: NEELA SANTOSH

TASK2:set up monitoring for cloud applications

This project implements centralized monitoring and alerting for a cloud-based application using Amazon CloudWatch to ensure high availability, performance visibility, and proactive incident response. The application is deployed on Amazon EC2 instances behind Elastic Load Balancing, with a relational database hosted on Amazon RDS. The primary objective of this implementation is to collect infrastructure and application-level metrics, configure threshold-based alerts, and build a centralized dashboard that provides a real-time operational overview of the system. Detailed monitoring was enabled on EC2 instances to obtain one-minute granularity metrics, allowing faster detection of anomalies. In addition to default metrics such as CPU utilization, network input/output, and disk operations, the CloudWatch Agent was installed on the EC2 instances to capture memory utilization, disk usage percentages, and application log files. This agent was configured using the CloudWatch Agent configuration wizard and deployed as a system service to ensure continuous metric streaming to CloudWatch.

Application logs were configured to stream into CloudWatch Logs through log groups and log streams, enabling centralized log management and analysis. A log retention policy of 30 days was applied to control storage costs while maintaining adequate history for troubleshooting. Metric filters were created to detect critical patterns such as HTTP 5XX server errors and application exceptions. These filters convert log events into measurable metrics that can be tracked and used to trigger alarms. CloudWatch Alarms were configured with specific thresholds to enable proactive alerting. For example, a High CPU Utilization alarm triggers when usage exceeds 80% for five consecutive minutes, while a High Memory Utilization alarm triggers when memory usage crosses 75%. Additional alarms were configured for low disk space and elevated HTTP 5XX error rates from the load balancer. All alarms are integrated with Amazon SNS to deliver real-time email notifications to the operations team, ensuring immediate awareness of potential issues.

A centralized CloudWatch Dashboard was created to provide a single-pane-of-glass view of application health. The dashboard includes widgets displaying EC2 CPU utilization, memory usage, disk utilization, network traffic, RDS CPU usage, database connections, load balancer request counts, and HTTP error rates. These visualizations allow operations teams to quickly identify performance bottlenecks, abnormal traffic spikes, or infrastructure constraints. By consolidating metrics from compute, database, and networking layers into one unified interface, the dashboard enhances situational awareness and accelerates root cause analysis. Overall, this monitoring implementation delivers comprehensive observability across the application stack, reduces mean time to detect incidents, and strengthens operational reliability in a production AWS environment.

<img width="1907" height="917" alt="Image" src="https://github.com/user-attachments/assets/40874b3a-1972-4daa-acc3-d88d8e67126b" />

<img width="1918" height="846" alt="Image" src="https://github.com/user-attachments/assets/6aefe69d-fcf4-4c86-8716-b25ffe9cf3c6" />

<img width="1592" height="593" alt="Image" src="https://github.com/user-attachments/assets/e50b9630-9456-4d9a-9a9f-1b879f594616" />
