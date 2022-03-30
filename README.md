# Banyan AWS Connector Module

Creates a Connector for use with [Banyan Security][banyan-security].

## Usage

```hcl
provider "aws" {
  region = "us-east-1"
}

module "aws_connector" {
  source                 = "banyansecurity/banyan-connector/aws"
  vpc_id                 = "vpc-0e73afd7c24062f0a"
  subnet_id              = "subnet-00e393f22c3f09e16"
  ssh_key_name           = "my-ssh-key"
  package_version        = "1.3.0"
  command_center_url     = ""
  api_key_secret
  connector_name
}
```


## Notes

[banyan-security]: https://banyansecurity.io
