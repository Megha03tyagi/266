# 🌐 Terraform Setup: NACL Rules

| Author         | Created on | Version | Last updated by | Last edited on | Reviewed By L0 | Reviewed By L1 | Reviewed By L2 |
|----------------|------------|---------|-----------------|----------------|----------------|----------------|----------------|
| Megha Tyagi  | 28-10-24   | 1.0     | Megha Tyagi   | 28-10-24       | -              | -              | -              |

## 📝 Table of Contents
1. [Purpose](#-purpose)
2. [Introduction](#-introduction)
3. [Key Features of NACL Rules](#-key-features-of-nacl-rules)
4. [Benefits of Using NACL Rules](#-benefits-of-using-nacl-rules)
5. [Steps for NACL Rules Setup](#-steps-for-nacl-rules-setup)
6. [Conclusion](#-conclusion)
7. [References](#-references)
8. [Contact Information](#-contact-information)

## 🎯 Purpose
This document provides a structured guide for creating Network Access Control List (NACL) Rules in AWS using static Terraform code, specifically tailored for managing network traffic and enhancing security within a development environment.


## 📖 Introduction
A Network Access Control List (NACL) in AWS allows users to define rules that control the inbound and outbound traffic within their Virtual Private Cloud (VPC), providing an additional layer of security and flexibility. This document outlines the necessary steps for setting up NACL Rules, emphasizing customization options and best practices for effective network management. By implementing NACL Rules, users can enhance the security posture of their cloud infrastructure and ensure efficient resource deployment while adhering to organizational policies.

## 🔑 Key Features of a NACL Rules

| Feature             | Description                                          |
|---------------------|------------------------------------------------------|
| Traffic Control      | Filters inbound and outbound traffic at the subnet level. |
| Stateless Rules      | Each request is evaluated against the rules without regard to previous requests. |
| Rule Prioritization  | Rules are evaluated in order, allowing for specific traffic handling. |
| Customization        | Allows users to define specific IP addresses, protocols, and ports. |
| Security Layer       | Provides an additional layer of security alongside Security Groups. |


## 🏆 Benefits of Using NACL Rules

- **Enhanced Security**: Provides an additional layer of security by controlling traffic at the subnet level, complementing existing Security Groups.
- **Fine-Grained Access Control**: Enables precise control over which IP addresses, protocols, and ports are allowed or denied access to resources.
- **Stateless Filtering**: Each request is evaluated independently, making it suitable for applications requiring specific traffic handling without the need for session tracking.
- **Scalability**: Easily adapts to changing network requirements by adding or modifying rules as needed.
- **Logging Capabilities**: Allows integration with AWS services for logging and monitoring traffic, facilitating better visibility and compliance.


## 🛠 Steps for NACL Rules Setup

#### Step 1: Initialize the Terraform Directory [Terraform code](https://github.com/mygurukulam-p10/infrastructure-repo/tree/Megha_Scrum_264/dev/Network)
- Run `terraform init` to prepare the directory and download required providers.
<img width="526" alt="image" src="https://github.com/user-attachments/assets/135e9c70-cf99-4105-acfd-c8304cc4743d">


#### Step 2: Format the Terraform Code
- Use `terraform fmt` to format and organize the Terraform configuration files.
<img width="264" alt="image" src="https://github.com/user-attachments/assets/3ffec4a9-0fdb-4d4c-93f1-cfbbb4ddbe22">


#### Step 3: Validate the Configuration
- Run `terraform validate` to check for syntax or configuration errors.
<img width="383" alt="image" src="https://github.com/user-attachments/assets/5f9b2fe7-8f07-4281-ac7c-fb5ebfc80221">


#### Step 4: Preview Infrastructure Changes
- Execute `terraform plan` to review resources that will be created.
<img width="790" alt="image" src="https://github.com/user-attachments/assets/98a5067e-e6ca-43de-ac02-7698368060c8">


#### Step 5: Apply the Configuration
- Run `terraform apply` to provision the VPC in AWS.
<img width="609" alt="image" src="https://github.com/user-attachments/assets/e90e4b07-4b73-4dc0-94e4-dcec9b3de1b1">

<img width="571" alt="image" src="https://github.com/user-attachments/assets/dd5f38c1-06e5-4ac2-ad0a-7834bc0b9cac">


## 🔚 Conclusion

In this document, we have outlined the essential steps for creating and managing Network Access Control List (NACL) Rules in AWS. By implementing NACL Rules, users can effectively control inbound and outbound traffic within their Virtual Private Cloud (VPC), enhancing security and providing fine-grained access control. The flexibility and scalability of NACL Rules make them a valuable component in establishing a robust and secure cloud infrastructure. By following the best practices and guidelines provided, users can ensure their network management strategies align with their organizational security policies and adapt to evolving requirements.


## 🔗 References

| Reference                    | Link                                                    |
|------------------------------|---------------------------------------------------------|
| Terraform AWS Provider       | https://www.dheeraj3choudhary.com/deploy-aws-nacl-inbound-amp-outbound-routes-security-group-amp-associate-with-subnet-using-terraform/|
| Dheeraj Tech|https://docs.aws.amazon.com/vpc/latest/userguide/nacl-rules.html|

## 📞 Contact Information
For questions, feedback, or further assistance, reach out to:

| Name          | Email address                        |
|---------------|-------------------------------------|
| Megha Tyagi | megha.tyagi.snaatak@mygurukulam.co |



