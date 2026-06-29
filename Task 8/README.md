# Task 8: Set IAM Roles and Policies

## Objective

The objective of this task was to understand and implement Identity and Access Management (IAM) in AWS by creating IAM user groups and assigning permissions using both AWS-managed policies and custom JSON policies.

---

## Tools Used

* AWS Identity and Access Management (IAM)
* AWS Management Console

---

## Task Description

This task involved securing cloud resources by creating IAM groups and policies to control access permissions. Both predefined AWS policies and custom policies were used to manage access rights.

---

## Steps Performed

### 1. Accessed AWS IAM Service

* Logged into the AWS Management Console.
* Opened the IAM (Identity and Access Management) dashboard.

### 2. Created an IAM User Group

* Navigated to **IAM → User Groups**.
* Created a new user group named:

  ```
  Task8Group
  ```

### 3. Attached AWS Managed Policy

* Selected and attached the AWS managed policy:

  ```
  AmazonS3FullAccess
  ```
* This policy provides full access to Amazon S3 services.

### 4. Created a Custom IAM Policy

* Navigated to **IAM → Policies → Create Policy**.
* Used the JSON editor to create a custom policy.

#### Custom Policy JSON:

```json
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Action": "s3:*",
            "Resource": "*"
        }
    ]
}
```

### 5. Created the Custom Policy

* Policy Name:

  ```
  Task8S3CustomPolicy
  ```
* Successfully created the customer-managed policy.

### 6. Attached the Custom Policy to the IAM Group

* Opened the **Task8Group**.
* Attached the newly created custom policy:

  ```
  Task8S3CustomPolicy
  ```

---

## Results

* Successfully created an IAM user group.
* Attached AWS-managed S3 permissions.
* Created and attached a custom IAM policy using JSON.
* Implemented access control management using AWS IAM.

---

## Screenshots Included

* IAM Dashboard
* IAM User Group Creation
* AWS Managed Policy Selection
* User Group Created
* Custom Policy JSON Editor
* Policy Review Page
* Policy Created Page
* Group Permissions Page

---

## Learning Outcomes

* Learned how AWS IAM manages authentication and authorization.
* Understood the difference between AWS-managed and customer-managed policies.
* Gained hands-on experience in creating and assigning IAM permissions.
* Learned how JSON policies define access permissions in AWS.

---

## Conclusion

This task provided practical experience in implementing access control mechanisms using AWS IAM. The successful creation and assignment of IAM roles and policies demonstrated the importance of identity and permission management in cloud security.
