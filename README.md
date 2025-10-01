# Source Code

- React, Node.js, Next.js, Tailwind CSS

# Tools

- Jenkins, Terraform, Docker, Kubernetes
- SonarQube (container), Trivy (container)
- (Optional) PostgreSQL, MongoDB, Redis/Memcached, RabbitMQ
- Helm, ArgoCD, Image Updater
- Valut, Promethus, Grafana

# Configure Files

- Dockerfile
- Kubernetes YAML files

# CI Pipeline Steps

- Checkout
- Build, Test
- GitLeaks
- OWASP Dependency Check
- SonarQube code analysis
- Trivy FS scan
- Create docker image
- Trivy image scan
- Push image to DockerHub/ECR
- Update CD repo with image tag
- Send Email notification

# CD Pipeline Steps

- ArgoCD update application automatically
- Send Email notification

# Pipeline Method

- Jenkins
- GitHub Action

# Steps - Jenkins

- Setup an EC2 instance as Jenkins server
- Install tools (AWS CLI, Docker, Jenkins)
- Setup Jenkins CI pipeline
- Test CI pipeline
- Setup EKS cluster as CD dev environment
- Setup Jenkins CD pipeline
- Test CD pipeline on the cluster

# Steps - GitHub Action

- Setup an EC2 instance as Jenkins server
- Install tools (AWS CLI, Docker, Jenkins, kubectl, helm)
- Setup Jenkins CI pipeline
- Test CI pipeline
- Setup EKS cluster as CD dev environment
- Install ArgoCD, Image Updater, Promethus, Grafana
- Setup Jenkins CD pipeline
- Test CD pipeline on the cluster

# CI repo structure



# Choices

- using implicit or explicit way to create PR for promoting dev->staging, staging->prod

- PR reviewers assignment (one line code / johnmanjiro13/auto-reviewer-assign)

# Questions

- Branch Protection Rules
