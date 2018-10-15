# token
*Step 1*

**First create personal access token by going to settings-Developer settings-generate new token.**

**Copy the token and run this command:**

*export TF_VAR_github_token="paste token here"

*Step 2*

**Override the name of the repo with this command:**

*variable export TF_VAR_repo=newname

*Step 3*

**Copy the following files and direcroties to your repo:**

**Gemfile, .kitchen.yml, teh whole test directory and testing.tfvars**

*Step 4*

**Run the following commands:**

Command | Explanation 
-------------- | -------------------------
terraform fmt | formats all terraform code
terraform init | initialize a working directory containing terraform configuration files
terraform plan | create an execution plan
terrafrom apply | applies the changes created by execution plan 
terraform destroy | destroy the terraform infrastructure
terrafrom apply | applies the changes created by execution plan 

*Step 5*

**For Linux users you need to update gemfile from 2.3.1 to 2.5.1**

**Run the following commands to update gemfile:**

*sudo apt-get install rbenv ruby-dev ruby-bundler


*Step 6*


**After that run the following commands:**

*bundle install - install the dependencies specified in your Gemfile

*bundle exec kitchen test
