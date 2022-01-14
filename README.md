# Repository for learning Terraform
This repository is returning an output value using the `Output Values` feature of Terraform OSS

## Instructions

### Prerequisites

- [X] [Terraform](https://www.terraform.io/downloads)

## How to Use this Repo

- Clone this repository:
```shell
git clone git@github.com:dlavric/terraform-output.git
```

- Go to the directory where the repo is stored and make sure the `main.tf` file is there too:
```shell
cd terraform-output
```

- Run `terraform init`, to download any external dependency
```shell
terraform init
```


This is the output of initializing the Terraform code:
```shell
Initializing the backend...

Initializing provider plugins...

Terraform has been successfully initialized!

You may now begin working with Terraform. Try running "terraform plan" to see
any changes that are required for your infrastructure. All Terraform commands
should now work.

If you ever set or change modules or backend configuration for Terraform,
rerun this command to reinitialize your working directory. If you forget, other
commands will detect it and remind you to do so if necessary.
```

- Apply the changes with Terraform
```shell
terraform apply
```

This is the output for applying the changes:
```shell
Changes to Outputs:
  ~ server = "1" -> "Hi, my name is Daniela"

You can apply this plan to save these new output values to the Terraform state, without changing any real infrastructure.

Do you want to perform these actions?
  Terraform will perform the actions described above.
  Only 'yes' will be accepted to approve.

  Enter a value: yes


Apply complete! Resources: 0 added, 0 changed, 0 destroyed.

Outputs:

server = "Hi, my name is Daniela"
```

- Destroy the instance
```shell
terraform destroy
```