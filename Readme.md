# 🌐 Terraform Setup: Load Balancer

| Author         | Created on | Version | Last updated by | Last edited on | Reviewed By L0 | Reviewed By L1 | Reviewed By L2 |
|----------------|------------|---------|-----------------|----------------|----------------|----------------|----------------|
| Megha Tyagi  | 28-10-24   | 1.0     | Megha Tyagi   | 28-10-24       | -              | -              | -              |

## 📝 Table of Contents
1. [Purpose](#-purpose)
2. [Introduction](#-introduction)
3. [Key Features of Load Balancer](#-key-features-of-load-balancer)
4. [Benefits of Using Load Balancer](#-benefits-of-using-load-balancer)
5. [Steps for Load Balancer Setup](#-steps-for-load-balancer-setup)
6. [Conclusion](#-conclusion)
7. [References](#-references)
8. [Contact Information](#-contact-information)

## 🎯 Purpose
This document provides a structured guide for creating a Load Balancer in AWS using static Terraform code, specifically tailored for distributing incoming application traffic and ensuring high availability within a development environment.

## 📖 Introduction
A Load Balancer in AWS enables users to distribute incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, and IP addresses, enhancing application availability and fault tolerance. This document outlines the necessary steps for setting up a Load Balancer, emphasizing customization options and best practices for effective traffic management. By implementing a Load Balancer, users can improve the responsiveness of their applications, ensure high availability, and optimize resource utilization while adhering to organizational performance and security requirements.


## 🔑 Key Features of a Load Balancer

| Feature                | Description                                          |
|------------------------|------------------------------------------------------|
| Traffic Distribution    | Balances incoming traffic across multiple targets to ensure even load. |
| High Availability       | Automatically redirects traffic to healthy instances, ensuring uptime. |
| Scalability            | Easily scales up or down to handle changes in traffic without downtime. |
| Health Checks          | Monitors the health of registered targets to route traffic only to healthy ones. |


## 🏆 Benefits of Using Load Balancer

- **Enhanced Availability**: Distributes incoming traffic across multiple targets, ensuring that applications remain accessible even during instance failures.
- **Improved Performance**: Optimizes resource utilization by balancing the load and reducing latency for end users.
- **Automatic Scaling**: Adjusts to fluctuating traffic patterns, allowing applications to scale seamlessly in response to demand.
- **Health Monitoring**: Continuously checks the health of targets and routes traffic only to healthy instances, improving application reliability.
- **Simplified SSL Management**: Offloads SSL/TLS termination from backend servers, simplifying certificate management and improving security.



## 🛠 Steps for Load Balancer Setup

#### Step 1: Initialize the Terraform Directory [Terroaform code](https://github.com/mygurukulam-p10/infrastructure-repo/tree/Megha_Scrum_265/dev/Network)
- Run `terraform init` to prepare the directory and download required providers.
<img width="459" alt="image" src="https://github.com/user-attachments/assets/96114204-7e41-43a7-a766-c9f94948fb00">


#### Step 2: Format the Terraform Code
- Use `terraform fmt` to format and organize the Terraform configuration files.
<img width="350" alt="image" src="https://github.com/user-attachments/assets/2f6795a8-c96b-4373-8a6b-f08bf95e9421">


#### Step 3: Validate the Configuration
- Run `terraform validate` to check for syntax or configuration errors.
<img width="355" alt="image" src="https://github.com/user-attachments/assets/8cfa5f15-ed61-46ad-9d4c-92869bc8a174">



#### Step 4: Preview Infrastructure Changes
- Execute `terraform plan` to review resources that will be created.
<img width="899" alt="image" src="https://github.com/user-attachments/assets/29fad50e-906a-4fa5-8289-8e7971c14a0c">



#### Step 5: Apply the Configuration
- Run `terraform apply` to provision the VPC in AWS.
<img width="758" alt="image" src="https://github.com/user-attachments/assets/66c32ac9-d521-416f-bc31-93e644c17d57">
<img width="920" alt="image" src="https://github.com/user-attachments/assets/d704d7f4-aa70-420b-88e8-904b89d03399">



## 🔚 Conclusion

In this document, we have outlined the essential steps for setting up a Load Balancer in AWS, emphasizing its critical role in distributing application traffic and enhancing availability. By leveraging the features and benefits of Load Balancers, users can improve application performance, ensure high availability, and optimize resource utilization within their cloud environments. Following the best practices outlined will help organizations effectively manage traffic, enhance security, and adapt to changing demands, ultimately leading to a more robust and resilient cloud infrastructure.


## 🔗 References

| Reference                    | Link                                                    |
|------------------------------|---------------------------------------------------------|
| AWS Load Balancer Documents  |https://docs.aws.amazon.com/elasticloadbalancing/latest/application/introduction.html|
|Terraform AWS Provider|https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/lb|

## 📞 Contact Information
For questions, feedback, or further assistance, reach out to:

| Name          | Email address                        |
|---------------|-------------------------------------|
| Megha Tyagi | megha.tyagi.snaatak@mygurukulam.co |




# 🌐 Terraform Setup: Route-53

| Author         | Created on | Version | Last updated by | Last edited on | Reviewed By L0 | Reviewed By L1 | Reviewed By L2 |
|----------------|------------|---------|-----------------|----------------|----------------|----------------|----------------|
| Megha Tyagi  | 28-10-24   | 1.0     | Megha Tyagi   | 28-10-24       | -              | -              | -              |

## 📝 Table of Contents
1. [Purpose](#-purpose)
2. [Introduction](#-introduction)
3. [Key Features of Route-53](#-key-features-of-route-53)
4. [Benefits of Using Route-53](#-benefits-of-using-route-53)
5. [Steps for Rout-53 Setup](#-steps-for-route-53-setup)
6. [Conclusion](#-conclusion)
7. [References](#-references)
8. [Contact Information](#-contact-information)

## 🎯 Purpose
This document provides a structured guide for creating Amazon Route 53 in AWS using static Terraform code, specifically tailored for managing domain name system (DNS) services and ensuring reliable routing of network traffic within a development environment.

## 📖 Introduction
Amazon Route 53 in AWS provides a scalable and highly available Domain Name System (DNS) web service that allows users to manage the routing of network traffic to various resources within their Virtual Private Cloud (VPC) and beyond. This document outlines the necessary steps for setting up Route 53, emphasizing customization options and best practices for effective DNS management. By implementing Route 53, users can enhance the reliability and efficiency of their applications, ensuring secure and optimal resource deployment while adhering to organizational policies and compliance requirements.


## 🔑 Key Features of a Route-53

| Feature            | Description                                          |
|--------------------|------------------------------------------------------|
| DNS Management      | Provides a reliable and scalable DNS service for domain names. |
| Traffic Routing     | Directs user requests to the appropriate endpoints based on routing policies. |
| Health Checks       | Monitors the health of resources and ensures traffic is routed only to healthy endpoints. |
| Global Availability  | Ensures high availability and low latency through a network of global DNS servers. |
| Routing Policies    | Supports various routing policies, including simple, weighted, latency-based, and geolocation routing. |


## 🏆 Benefits of Using Route-53

- **High Availability**: Amazon Route 53 is designed for reliability, ensuring that DNS queries are answered with low latency and high availability through its global network of DNS servers.
- **Scalability**: Easily scales to accommodate increasing traffic demands, handling millions of requests without compromising performance.
- **Traffic Management**: Offers advanced routing policies, allowing users to direct traffic based on performance, geographic location, or even health status of endpoints.
- **Integrated Health Checks**: Automatically monitors the health of application endpoints and routes traffic only to healthy resources, improving application resilience.
- **Cost-Effective**: Pay-as-you-go pricing model ensures that users only pay for the resources they utilize, making it cost-effective for various application scales.

## 🛠 Steps for Rout-53 Setup

#### Step 1: Initialize the Terraform Directory [Terroaform code](https://github.com/mygurukulam-p10/infrastructure-repo/tree/Megha_Scrum_266/dev/Network)
- Run `terraform init` to prepare the directory and download required providers.
<img width="506" alt="image" src="https://github.com/user-attachments/assets/7ab6dd09-dc61-4991-9d30-a22b0f678ce1">



#### Step 2: Format the Terraform Code
- Use `terraform fmt` to format and organize the Terraform configuration files.
<img width="278" alt="image" src="https://github.com/user-attachments/assets/56ad4e89-f86f-45d8-985e-464099f17056">



#### Step 3: Validate the Configuration
- Run `terraform validate` to check for syntax or configuration errors.
<img width="314" alt="image" src="https://github.com/user-attachments/assets/2b95be11-d750-49cc-9c13-d7b7862f1b37">



#### Step 4: Preview Infrastructure Changes
- Execute `terraform plan` to review resources that will be created.
<img width="756" alt="image" src="https://github.com/user-attachments/assets/0d025208-4ccd-4c89-9d3d-b9e47676da28">



#### Step 5: Apply the Configuration
- Run `terraform apply` to provision the VPC in AWS.
<img width="760" alt="image" src="https://github.com/user-attachments/assets/4f06a18c-3eed-4723-9300-11295212cc48">
<img width="639" alt="image" src="https://github.com/user-attachments/assets/c3f98b33-1613-4e5b-829a-0c6d6dda055e">



## 🔚 Conclusion
In this document, we have outlined the essential steps for setting up Amazon Route 53 in AWS, highlighting its critical role in managing DNS services and routing network traffic effectively. By leveraging the features and benefits of Route 53, users can enhance the availability, performance, and resilience of their applications while ensuring secure and efficient resource deployment. Following the best practices and customization options discussed will help organizations optimize their DNS management strategies, align with business objectives, and adapt to evolving traffic demands, ultimately leading to a robust cloud infrastructure.



## 🔗 References

| Reference                    | Link                                                    |
|------------------------------|---------------------------------------------------------|
| Terraform AWS Provider       | https://registry.terraform.io/modules/terraform-aws-modules/route53/aws/latest|
| AWS Route-53 Documentation|https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/Welcome.html|

## 📞 Contact Information
For questions, feedback, or further assistance, reach out to:

| Name          | Email address                        |
|---------------|-------------------------------------|
| Megha Tyagi | megha.tyagi.snaatak@mygurukulam.co |


=======
# Commands To run this 


terraform init

terraform fmt

terraform validate

terraform plan 

terrafom apply