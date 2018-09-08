# Terraform Provisioner

Terraform not only helps us in infrastructure creation and management but also in provisioning them during resource creation or deletion. Terraform uses provisioners for this. Provisioners are used to executing scripts on a local or remote machine as part of resource creation or deletion. Provisioners are similar to EC2 instance user data scripts that only run once on the creation and if it fails terraform marks it tainted. A tainted resource is one which is planned for destruction on next terraform apply. Terraform doesn't run these scripts multiple times. If we want more flexibility then we must use a configuration management system like ansible to properly provision the instance.

Commands used:

terraform init : Initialize a Terraform working directory

terraform plan : Generate and show an execution plan

terraform apply : Builds or changes infrastructure

terraform destroy : Destroy Terraform-managed infrastructure
