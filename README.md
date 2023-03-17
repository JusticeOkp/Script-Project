# Deploying a ec2 instance with terraform and use a bash script to pull the ec2 metrics.

This is a project using a bash script to pull ec2 metrics, deployed using terraform. 
#
## Steps:
1. Create a new directory for the project on terraform and intialize the new terraform configuration.
2. Open the Terraform configuration file and define the AWS provider and the EC2 instance(T2-mirco).
3. Validate the configuration using "terraform validate", Once everything is correct run an "apply" to create the Ec2 instance.
4. Create a bash script to pull its metrics using AWS CLI commands.
5. Save the bash script and to use it in the terraform configuration use "Terraform remote-exec" provisioner to run the script on the ec2 instance.
6. Finally, run a "Terraform apply" to provision your EC2 instance and run your bash script.
