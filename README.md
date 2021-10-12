# tf-aws-minecraft
Terraform backed Minecraft server for aws housed in spot fleet.


 ## Overview

 * This is a completely self configured self deploying ts3 server for aws cloud

 ## Prerequisites
 * A basic knowledge of terraform , how to apply and run it.
 * A basic understanding of how to configure / setup and use aws cli commands.  You will need to setup appropriate profile
 * Linux experience and AWS account to deploy into.

 NB
 * It is recommended that you setup/and use a remote state.

 ## Versions

 See change log for specifics.

  * 0.#.# >= Pre-Alpha testing phase

 ## Usage

 ### Setup
 * Checkout the code. Enter the `backend-state` directory and run `terraform init && terraform apply`. This will create the backend remote state objects. Take note of the bucket name output.
 * Then simply run `terraform apply` in the parent terraform directory and provide the variables required. It will create the rest.
 * Or include the variables in a parameter file like `terraform apply --var-file=params/default.tfvars`

 ### Post infra deployment
 * ???

### Additional Information / Steps you can do
 * ????

 ## Future features
* Ability to use spot fleet setup / asg's

 # !!!! DISCLAIMER !!!!

 All code is currently designed to run within aws. All costs are down to the responsibility of the aws account owner. If you dont know/understand what this is deploying. Dont deploy it. There may be running costs involved with elastic ips/storage/keypairs that you as the aws account owner would be responsible for.
