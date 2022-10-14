# packer-demo
HashiCorp Packer Demo

## How to create AWS EC2 AMI

Source: https://learn.hashicorp.com/tutorials/packer/aws-get-started-build-image?in=packer/aws-get-started

In this example Packer uses the Packer Amazon AMI builder plugin.

```
$ cd hashicorp-learn/
$ packer init .
$ packer fmt .
$ packer validate .
$ export AWS_PROFILE="my_profile_name"
$ packer build aws-ubuntu.pkr.hcl
```

If `~/.aws/credentials` contains multiple profiles, `AWS_PROFILE` needs to be set to the name of the profile we want to use.
