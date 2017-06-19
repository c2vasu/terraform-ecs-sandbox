# Terraform AWS ECS Sandbox

* Terraform AWS ECS sandbox to build and manage containers.

# Demo overview
1. create ECR using terraform - myapp
2. Get ECR url - ecr-id.dkr.ecr.eu-west-1.amazonaws.com/myapp
3. Build and tag docker image - docker build -t ecr-id.dkr.ecr.eu-west-1.amazonaws.com/myapp:1 .
4. Login to ECR - aws ecr get-login
5. Push docker tagged image to ECR - docker push ecr-id.dkr.ecr.eu-west-1.amazonaws.com/myapp:1
