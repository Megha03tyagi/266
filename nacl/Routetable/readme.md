# 🌐 Terraform Setup: Route Table

| Author         | Created on | Version | Last updated by | Last edited on | Reviewed By L0 | Reviewed By L1 | Reviewed By L2 |
|----------------|------------|---------|-----------------|----------------|----------------|----------------|----------------|
| Megha Tyagi  | 28-10-24   | 1.0     | Megha Tyagi   | 28-10-24       | -              | -              | -              |

## 📝 Table of Contents
1. [Purpose](#-purpose)
2. [Introduction](#-introduction)
3. [Key Features of Route Table](#-key-features-of-route-table)
4. [Benefits of Using Route Table](#-benefits-of-using-route-table)
5. [Steps for Rout Table Setup](#-steps-for-rout-table-setup)
6. [Conclusion](#-conclusion)
7. [References](#-references)
8. [Contact Information](#-contact-information)

## 🎯 Purpose
This document provides a structured guide for creating a Route Table in AWS using static Terraform code, specifically tailored for managing network traffic within a development environment.

## 📖 Introduction
A Route Table in AWS enables users to control the routing of network traffic within their Virtual Private Cloud (VPC), allowing for secure and efficient resource deployment. This document outlines the necessary steps for setting up a Route Table, emphasizing customization and best practices for network management.

## 🔑 Key Features of a Route Table

| Feature         | Description                                          |
|-----------------|------------------------------------------------------|
| Routing Control  | Directs traffic between subnets and the internet.    |
| Static Routes    | Allows manual configuration of routes for specific destinations. |
| Propagation      | Supports automatic route propagation from Virtual Private Gateways. |
| Association      | Can be associated with multiple subnets for flexible traffic management. |
| Overriding Routes| Ability to override default routes for more precise control. |

## 🏆 Benefits of Using Route Table

- **Enhanced Security**: Provides isolated networking with the ability to define public and private subnets, improving overall security.
- **Scalability**: Easily adapts to changing requirements, allowing for the addition of new subnets and routes as needed.
- **High Availability**: Supports multiple Availability Zones, ensuring resilience and fault tolerance in network traffic management.


## 🛠 Steps for Rout Table Setup

#### Step 1: Initialize the Terraform Directory [Terraform Code](https://github.com/mygurukulam-p10/infrastructure-repo/tree/Megha_Scrum_262/dev/Network)
- Run `terraform init` to prepare the directory and download required providers.
<img width="577" alt="image" src="https://github.com/user-attachments/assets/df2f742a-00a4-4d3b-b605-ddc3a7db7c1d">

#### Step 2: Format the Terraform Code
- Use `terraform fmt` to format and organize the Terraform configuration files.
<img width="341" alt="image" src="https://github.com/user-attachments/assets/9456ec3e-923a-487a-a192-2013c1708131">

#### Step 3: Validate the Configuration
- Run `terraform validate` to check for syntax or configuration errors.
<img width="341" alt="image" src="https://github.com/user-attachments/assets/ff31c7da-22fc-41d9-87be-3b07b64b381b">

#### Step 4: Preview Infrastructure Changes
- Execute `terraform plan` to review resources that will be created.
<img width="835" alt="image" src="https://github.com/user-attachments/assets/ad458ce9-81ac-48d2-8d2d-9cee4898ed81">

#### Step 5: Apply the Configuration
- Run `terraform apply` to provision the VPC in AWS.
<img width="857" alt="image" src="https://github.com/user-attachments/assets/9d325555-e2b1-4e6b-9992-06a9d0c36a30">
<img width="674" alt="image" src="https://github.com/user-attachments/assets/0903225d-fc71-4ab2-bed0-4a1e17857a0f">


## 🔚 Conclusion
This document provides a concise guide for creating a Route Table in AWS using Terraform, establishing a critical component for managing network traffic within a Virtual Private Cloud (VPC) while ensuring security and flexibility in cloud infrastructure.


## 🔗 References

| Reference                    | Link                                                    |
|------------------------------|---------------------------------------------------------|
| Terraform AWS Provider       | https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/vpc_endpoint_route_table_association|
| AWS Route Table Documentation|https://docs.aws.amazon.com/vpc/latest/userguide/RouteTables.html|

## 📞 Contact Information
For questions, feedback, or further assistance, reach out to:

| Name          | Email address                        |
|---------------|-------------------------------------|
| Megha Tyagi | megha.tyagi.snaatak@mygurukulam.co |


