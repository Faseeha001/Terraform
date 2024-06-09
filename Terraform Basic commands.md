# Terraform Basic Commands Guide

## Introduction
This README provides an overview of basic Terraform commands used for managing infrastructure as code (IaC) with Terraform.

## Prerequisites
Before using Terraform, ensure you have the following:
- Terraform installed on your system. Installation instructions can be found [here](https://learn.hashicorp.com/tutorials/terraform/install-cli).
- Access to a cloud provider (e.g., AWS, Azure, Google Cloud).
- Provider credentials or access keys configured for your cloud provider.

## Usage
To use Terraform, navigate to your Terraform configuration directory containing your `.tf` files and execute the following commands:

### 1. `terraform init`
Initialize a Terraform configuration directory to install provider plugins and modules.

<img width="835" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/1024f761-057f-49a3-a9c6-f3274c7c3d3e">


### 2. `terraform plan`
Generate an execution plan showing the changes Terraform will make to your infrastructure. This command is often used to review planned changes before applying them.

<img width="750" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/86e52eff-a7fd-426a-a7e1-4556d94c6c45">

### 3. `terraform apply`
Apply the changes described in the Terraform execution plan. This command creates, updates, or deletes resources according to your configuration.

<img width="750" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/01b56cd8-1aa7-4d6a-9522-b69ac20ae4fd">

### 4. `terraform destroy`
Destroy all resources managed by Terraform. Use this command with caution, as it irreversibly deletes infrastructure.

<img width="819" alt="image" src="https://github.com/Faseeha001/Terraform/assets/169563689/f74bb4b3-ed06-47a8-99a7-6b1e8cc7db53">


### 5. `terraform validate`
Validate the syntax and consistency of your Terraform configuration files. This command checks for errors in your configuration.

### 6. `terraform fmt`
Format your Terraform configuration files to ensure consistent styling and formatting.

### 7. `terraform show`
Show the current state of your infrastructure managed by Terraform. This command provides a detailed view of resources and their attributes.

### 8. `terraform state`
View or manage Terraform state. This command is useful for advanced state management operations.

## Additional Resources
For more information on Terraform commands and usage, refer to the [Terraform CLI documentation](https://www.terraform.io/docs/cli/index.html).

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
