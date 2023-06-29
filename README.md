# terraform-module-vpc

## Usage:

```hcl
module "ec2" {
  source  = "zazuwka/vpc/module"
  version = "0.0.1"
  region = "us-east-2"
  vpc_main_cidr_block = "10.0.0.0/16"
  vpc_subnet1_cidr_block = "10.0.1.0/24"
  vpc_subnet2_cidr_block = "10.0.2.0/24"
  vpc_subnet3_cidr_block = "10.0.3.0/24"
  vpc_private1_cidr_block = "10.0.101.0/24"
  vpc_private2_cidr_block = "10.0.102.0/24"
  vpc_private3_cidr_block = "10.0.103.0/24"
  default_cidr_block = "0.0.0.0/0"
  key_name = "yo-key"
  key_file = "~/.ssh/id_rsa.pub"
  instance_type = "t2.micro"

}
```