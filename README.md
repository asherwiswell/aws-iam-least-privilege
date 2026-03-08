# aws-iam-least-privilege


## Overview

This project demonstrates how to implement the principle of least privilege using AWS IAM. 
An IAM user was created and granted restricted access to a specific S3 bucket using a custom IAM policy. 
The project shows how permissions control access to AWS resources and how incorrect access attempts are denied.

## Architecture

This project uses the following components:

- IAM User
- Custom IAM Policy
- Amazon S3 Bucket

The IAM user is allowed to view and download objects from a single S3 bucket but is denied access to other AWS services.

## Technologies Used

- AWS IAM
- Amazon S3
- AWS Management Console
- JSON policy language

## Security Objective

The objective of this project is to demonstrate the principle of least privilege. 
The IAM user is granted only the minimum permissions required to access a specific S3 bucket.

## Deployment Steps

1. Created a new IAM user.
2. Enabled AWS Management Console access.
3. Created a custom IAM policy allowing access to a specific S3 bucket.
4. Attached the policy to the IAM user.
5. Logged in as the IAM user to verify permissions.


---

# Testing Access Controls

This section is **very good for portfolios**.

## Testing Access Controls

The IAM user was tested to verify correct permission behavior.

Allowed actions:
- View the S3 bucket
- Download objects from the bucket

Denied actions:
- Launch EC2 instances
- Access other S3 buckets
- Modify bucket permissions

## Screenshots

### IAM User Created
![IAM User](screenshots/iam-user.png)

### Custom Policy
![IAM Policy](screenshots/iam-policy.png)

### Access Denied Example
![Access Denied](screenshots/access-denied.png)




