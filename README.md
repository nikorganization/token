# token

First create personal access token by going to settings-Developer settings-generate new token. 
Copy the token and run this command: export TF_VAR_github_token="paste token here"
Override the name of the repo with this command: variable export TF_VAR_repo=newname

Copy the following files and direcroties to your repo:
Gemfile, .kitchen.yml, teh whole test directory and testing.tfvars

Run the following commands:
terraform fmt - formats all terraform code
terraform init - initialize a working directory containing terraform configuration files
terraform plan - create an execution plan
terrafrom apply - applies the changes created by execution plan 
terraform destroy - destroy the terraform infrastructure.
terrafrom apply - applies the changes created by execution plan 

For Linux users you need to update gemfile from 2.3.1 to 2.5.1
Run the following commands:
sudo apt-get install rbenv ruby-dev ruby-bundler

After that run teh following commands:
bundle install
bundle exec kitchen test
