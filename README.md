# terraform-flux-github

Terraform module to deploy an AWS backend with restrictive policies.

## How to use this module with Terragrunt

```hcl
terraform {
  source = "tfr:///yivolve/backend/aws?version=<tag version>"
}

<optional terragrunt's configuration goes here>

inputs = {
  path = <path>
  ...rest of the inputs go here
}

```

> [!TIP]
> If by any change you get locked out from your s3 bucket and dynamodb table run the commands below from the cloudshell using your root account:
>
>```bash
> aws s3api delete-bucket-policy --bucket <bucket name>
> aws dynamodb delete-resource-policy --resource-arn <table arn>
>```
