# Microservices App Repository

Welcome to the Microservices App repository! This repository contains code and configurations for a simple microservices-based application along with Terraform scripts for Cloud Functions.

## Repository Structure

The repository is organized as follows:

microservices-app/
|-- README.md
|-- docs/
| |-- architecture_diagram.png
| |-- deployment_guide.md
|-- microservices/
| |-- service1/
| |-- Dockerfile
| |-- app/
| |-- main.py
| |-- k8s/
| |-- deployment.yaml
| |-- service2/
| |-- Dockerfile
| |-- app/
| |-- main.py
| |-- k8s/
| |-- deployment.yaml
| |-- k8s/
| |-- ingress.yaml
| |-- secrets.yaml
|-- scripts/
| |-- deploy.sh
|-- terraform/
| |-- modules/
| |-- cloudfunctions/
| |-- main.tf
| |-- variables.tf
| |-- outputs.tf
| |-- environments/
| |-- dev/
| |-- main.tf
| |-- variables.tfvars
| |-- prod/
| |-- main.tf
| |-- variables.tfvars
|-- .gitignore



## Setting Up Microservices Application

1. **Clone the Repository:**
   ```bash
   git clone <repository_url>
   cd microservices-app

Build and Deploy Microservices:

Navigate to the microservices folder.
Follow instructions in the service1 and service2 directories to build Docker images and deploy to Kubernetes.
Kubernetes Ingress and Secrets:

Configure the Ingress and Secrets in the k8s folder.
Update the paths and configurations according to your requirements.
Deploy Microservices:

Execute the deployment script in the scripts folder.

cd scripts
./deploy.sh


Explore Documentation:

Check the docs folder for an architecture diagram (architecture_diagram.png) and deployment guide (deployment_guide.md).

Setting Up Terraform for Cloud Functions
Navigate to the Terraform Directory:
cd terraform

Configure Modules:

Update the configurations in modules/cloudfunctions/main.tf according to your Cloud Functions requirements.
Set Up Environments:

Navigate to environments/dev or environments/prod and configure the environment-specific Terraform files and variables.
Initialize and Apply Terraform:

Initialize Terraform in the respective environment.
terraform init

Apply the Terraform configuration.
terraform apply -var-file=variables.tfvars


Notes
Ensure you have the necessary dependencies installed (Docker, kubectl, Terraform).
Modify placeholder values in files as needed.
Refer to individual service, Kubernetes, and Terraform documentation for detailed configurations.
