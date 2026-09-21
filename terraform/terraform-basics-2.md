# Terraform As Tool.

1. Terraform ia s tool for building, changing and versioning infrastructure safely and efficiently.
2. It enables application software best practice to infrastructure.
3. It is compatible with many clouds and services.
4. Terraform is provisioning focus tool, Asible is a configuration focus tool, while Kubernetes is an orchestration tool. Terraform can work with both Ansible and Kubernetes.
5. Terraform State and Terraform Config are made up of Terraform Core.

# State File

1. `State File` Terraform sentation of the world.
2. `Json File` Contains information about every resources and data object.
3. Contains Sensitive information (eg database password).
4. Can be stored locally or remotely. Remote Backend (via Terraform Cloud or Amazon Simple Storage Service) enables Sensitive data encryption, Collaboration and Automation. But it increases complexity.
