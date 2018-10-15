# name of repo here

What this repo does

## pre-requirements

- create personal access ![token](https://github.com/settings/tokens
- run `export TF_VAR_github_token=<token generated>`
- optionally, you can override the repo with `export TF_VAR_repo=<name>`
- this repo requires bundler, if you are in ubuntu linux, you can use:
```
sudo apt-get install -y ruby-bundler
```

## create a new repo


Command | Explanation 
-------------- | -------------------------
terraform init | initialize a working directory containing terraform configuration files
terraform plan | create an execution plan
terrafrom apply | applies the changes created by execution plan 
terraform destroy | destroy the terraform infrastructure

## test

```
bundle install # install the dependencies specified in Gemfile
bundle exec kitchen test
```
