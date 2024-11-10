# Exercise 1: Multi-Cloud Infrastructure Deployment with Terraform and Ansible

### Objective: 
Deploy a multi-cloud setup across AWS and OCI using Terraform, creating resilient infrastructure for disaster recovery.


### Requirements:

1. Use Terraform with appropriate providers to do the following:
    - **Create primary Region on AWS**: Create a VPC with one public & two private subnets, two EC2 instances on the private subnets one for web/app server and the second for MongoDB, also create an Application Load Balancer.

    - **Secondary Region on OCI**: Deploy equivalent infrastructure using the appropriate OCI resources for networking, compute, and load balancing.

    - **Connect the two providers using VPN**: Create the required nectwork components (Customer Gateway, Virtual Private Gateway, Dynamic Routing Gateway, ...) to connect the both VPC & VCN and preparing the connection between MongoDB instances.

    - **Enable monitoring Setup**: Deploy CloudWatch (AWS) and Monitoring (OCI) for infrastructure metrics and alerts.

2. Use Ansible to create the following:
    - **Create a dummy app connects to db**: Create an application using any language/framework that connects to mongodb (add CURD operations capabilities is plus).
    - **Prepare the web servers**: Deploy the app using docker behind Nginx on the web server with minimum 2 replicas.
    - **Deploy MongoDB on DB server**: Install MongoDB on both servers (AWS instance & OCI VM) then create replicaSet between them (add encyption key is plus).

### Tasks:

1. Create AWS Diagram
2. Create the required files with proper repo strucuture and push it to this [repo](https://github.com/EmadGKamel/multi-cloud-infrastructure-deployment-with-terraform-and-ansible). Don't forget the gitignore file

### Deliverables:

- AWS diagram on PDF format.

- Ansible & TF files pushed to mentioned repo.

- URL/Screenshots showing the website accessible via the CloudFront URL.
