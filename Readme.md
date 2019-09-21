# Introduction
A quick way to spin up a Kube cluster in digitalocean from the shell

# Prerequisites
Fill your `.env` file with the following details
```
export TF_VAR_do_token=<your DO token>
export TF_VAR_do_cluster_name=<name of your kube cluster>
```

You also need terraform installed and kubectl (I use version 1.16)

# Setup
```
. ./env
terraform plan
terraform apply
sh ./get_config.sh
```

# Destroy
```
terraform destroy
```
