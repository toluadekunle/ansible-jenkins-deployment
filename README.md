Ansible Jenkins Deployment on AWS EC2
This project contains Ansible playbooks and roles to automate the deployment of Jenkins on AWS EC2 instances. It aims to provide a consistent, scalable, and repeatable Jenkins setup across different environments.

Prerequisites
Before running the playbook, ensure you have the following:

AWS Setup:

An AWS account with appropriate permissions to create and manage EC2 instances.
AWS CLI installed and configured with the necessary AWS credentials.
Ansible Setup:

Ansible installed (Version 2.9 or above recommended).
Necessary Ansible dependencies installed. This can typically be done using pip install ansible[azure].
SSH Key Pair:

Ensure you have an SSH key pair set up and the private key is available on the machine where you're running the playbook. This key will be used to SSH into the EC2 instances.

Step-by-step Guide
1: Clone the Repository:

git clone https://github.com/toluadekunle/ansible-jenkins-deployment.git
cd ansible-jenkins-deployment

2: Configure AWS Credentials:
If not already done, configure your AWS CLI with the required credentials:

aws configure

3:Run the Playbook:

ansible-playbook jenkins_install.yml

4:Access Jenkins:
After successfully running the playbook, you can access Jenkins using the EC2 instance's public IP:

http://<Your-EC2-Instance-IP>:8080
