

# Creating AWS IAM User

This guide walks you through the process of creating a user in AWS using IAM (Identity and Access Management). IAM allows you to manage access to AWS services securely.

## Prerequisites

- An AWS account with administrative privileges.
- Access to the AWS Management Console.

## Steps to Create IAM User

1. **Sign in to the AWS Management Console**

    Go to the [AWS Management Console](https://aws.amazon.com/console/) and sign in using your AWS account credentials.

2. **Navigate to the IAM Service**

    Once logged in, navigate to the IAM (Identity and Access Management) service. You can find it by searching for "IAM" in the AWS Management Console search bar or by locating it under "Security, Identity, & Compliance" in the services menu.

3. **Access IAM Users**

    In the IAM dashboard, select "Users" from the sidebar menu.
   <img width="683" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/4dc1e0be-beb9-4369-ad7d-242cdeef8f91">

5. **Choose/Create User**

    - Choose an existing user for which you want to generate access keys or create a new user by clicking on the "Add user" button.

6. **Set Permissions**

    Ensure the user has the necessary permissions attached to them through IAM policies. These permissions will determine what actions the user can perform in AWS.

7. **Generate Access Keys**

    - Once you've selected or created a user, go to the "Security credentials" tab for that user.
    - Under the "Access keys" section, click on the "Create access key" button.

8. **Copy Access Key**

    - Once the access key is generated, you'll see the Access Key ID and Secret Access Key. Copy these credentials to a secure location. Note that the Secret Access Key will be displayed only once, so make sure to store it securely.

9. **Configure Access Keys**

    Use the Access Key ID and Secret Access Key to configure AWS CLI, SDKs, or other tools that require AWS credentials for programmatic access to AWS services.

10. **Secure Access Keys**

    Treat your access keys like passwords. Keep them secure and avoid sharing them unnecessarily. If you believe your access keys have been compromised, you can rotate them in the IAM console.



