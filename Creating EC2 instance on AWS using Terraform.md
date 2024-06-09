# Creating EC2 Instance with Terraform on Ubuntu

This guide outlines the steps to create an EC2 instance using Terraform on Ubuntu.

## Step 1: Install Terraform

<a href="https://github.com/Faseeha001/Terraform/blob/main/Terraform%20Installation%20on%20LINUX.md">Terraform Installation on Linux  </a>

## Step 2 : Set Up AWS Credentials

<a href="https://github.com/Faseeha001/AWS/blob/main/Create%20AWS%20IAM%20user%20.md">Set Up AWS Credentials </a>

## Step3 : Write Terraform Configuration

1. Create a new directory for Terraform configuration files
  ** mkdir terraform_ec2
   cd terraform_ec2**

<img width="861" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/fcc955a0-6c31-4ac2-9191-7e6a1d9c0e90">

2. Create a file named main.tf and add the following Terraform configuration:
**nano main.tf**
<img width="397" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/9c775d3a-8b54-4f7c-bab2-67bc856fd7b6">

Change the value of "region" if you want to create the instance in some other region 

3. Create 'variables.tf' which contains the declaration and definition of the variables

**nano variables.tf**

<img width="568" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/6e9efb83-e595-4c40-b564-0a494a5b456e">

4.Create 'terraform.tfvars' which contains the definition of access_key and secret_key variables defined in the above file. We have kept the declaration of these 2 variables in 'terraform.tfvars' file.

**nano terraform.tfvars**

<img width="669" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/171efcbb-7413-49b5-ab8e-76c94076ef40">

## step4 : Create an EC2 Instance using the Terraform configuration files

1. The first command to be used is 'terraform init'. This command downloads and installs plugins for providers used within the configuration. In our case it is AWS.

**terraform init**

<img width="848" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/d19cca42-2761-4e8c-b7b9-c955b5d33861">

2.The second command to be used is 'terraform plan'. This command is used to see the changes that will take place on the infrastructure.

**terraform plan**

<img width="852" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/5dfa5b79-3c9c-466d-ac16-2cef8a24da72">

3.'terraform apply' command will create the resources on the AWS mentioned in the main.tf file. You will be prompted to provide your input to create the resources.

**terraform apply**

When you execute the above command,  you can see that 1 new resource has been added and 0 has been destroyed in the output.

<img width="689" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/72724f85-9007-4906-832c-cf2f5f92c650">


You can go to the AWS EC2 console to verify if theEC2 instance is created or no

<img width="582" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/8324f778-1936-4b42-960e-6926c2e44f87">

4.Delete the created EC2 Instance using Terraform

If you no longer require resources you created using the configuration mentioned in the main.tf file, You can use the "terraform destroy" command to delete all those resources.

**terraform destroy**

<img width="724" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/0cf5dce1-92d2-44ec-be9c-52697b075964">

<img width="820" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/655cc504-b90d-4f40-afcc-fe4637255b4f">


