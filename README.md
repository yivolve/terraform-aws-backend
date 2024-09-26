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
