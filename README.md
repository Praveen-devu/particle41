# Task 2 - Terraform and Cloud: create the infrastructure to host your container.

## Prerequisites

Please ensure the following are installed on your local machine:

Terraform 

AWS CLI

VS Code

Make sure your docker is running in the entire process

Access to an AWS account with sufficient permissions

### AWS Authentication

You must authenticate to AWS before running terraform.

### Option 1: Using AWS CLI or using command prompt

aws configure

It will task the following details, give your access key and secret key

AWS Access Key ID: "your-access-key"

AWS Secret Access Key: "your-secret-key"

Default region name: us-west-1

Default output format: json


### create a directory ex: app

mkdir app

cd app

# 1. Clone the Repository
git clone https://github.com/visala29/particle41.git 

cd particle41

checkout to TerraformProject branch

open the terraform.tfvar files in vscode editor and 

update your "your-dockerhub-username"/"your-image-name":latest in terraform.tfvar file

ex: container_image = "praveen360/my-app:latest"


# 2. Build the Docker Image

docker build -t "your-dockerhub-username"/"your-image-name" .

docker push "your-dockerhub-username"/"your-image-name"

# 3. creating infrastructure using Terraform

terraform init

terraform plan

terraform apply it will create all the resources.

you will get below response: Apply complete! Resources: 27 added, 0 changed, 0 destroyed.

use terraform destroy for deleting the resources.
