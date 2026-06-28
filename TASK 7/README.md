# Task 7: Monitor Cloud Resources Using AWS CloudWatch

## Objective
The objective of this task is to monitor cloud resources using Amazon CloudWatch by tracking EC2 instance metrics and configuring alarms for resource utilization.

---

## Services Used
- Amazon EC2
- Amazon CloudWatch
- Amazon SNS (for notifications)

---

## EC2 Instance Details
- Instance Name: Task3-Instance
- Instance ID: i-07244511419126baa
- AWS Region: Europe (Stockholm)

---

## Monitoring Metric
The following metric was monitored:

- Metric Name: CPUUtilization
- Namespace: AWS/EC2
- Statistic: Average
- Period: 5 Minutes

---

## Alarm Configuration

A CloudWatch alarm was created with the following settings:

| Parameter | Value |
|-----------|-------|
| Alarm Name | Task7-CPUUtilization-Alarm |
| Metric | CPUUtilization |
| Threshold | Greater than 80% |
| Evaluation Period | 1 Datapoint within 5 minutes |
| Action | SNS Notification |
| State | Insufficient Data / OK |

---

## Steps Performed

### Step 1: Open Amazon CloudWatch
- Logged into AWS Management Console.
- Opened the CloudWatch service.

### Step 2: Access EC2 Metrics
- Navigated to:
  ```
  CloudWatch → Metrics → EC2
  ```
- Selected the EC2 instance metrics.
- Chose the CPUUtilization metric.

### Step 3: Analyze CPU Utilization
- Viewed the CPU utilization graph of the EC2 instance.
- Verified that CloudWatch was collecting monitoring data.

### Step 4: Create CloudWatch Alarm
- Selected the CPUUtilization metric.
- Configured an alarm with a threshold of 80%.
- Set the evaluation period to 5 minutes.

### Step 5: Configure Notifications
- Configured Amazon SNS notifications.
- Enabled alarm actions.

### Step 6: Review and Create Alarm
- Reviewed the alarm configuration.
- Successfully created the CloudWatch alarm.

### Step 7: Verify Alarm
- Verified the alarm under:
  ```
  CloudWatch → Alarms
  ```
- Confirmed that the alarm was successfully created.

---

## Screenshots Included

- CPUUtilization Graph
- Create Alarm Configuration
- Configure Actions
- Alarm Details
- Alarm Preview
- Alarm Created Successfully
- CloudWatch Alarm Dashboard

---

## Result

Successfully monitored AWS EC2 resources using Amazon CloudWatch and created a CPU utilization alarm to monitor system performance and resource utilization.
