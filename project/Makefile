virginia:
	terraform workspace new virginia || terraform workspace select virginia
	terraform init
	terraform apply --var-file regions/virginia.tfvars --auto-approve

oregon:
	terraform workspace new oregon || terraform workspace select oregon
	terraform init
	terraform apply --var-file regions/oregon.tfvars --auto-approve

california:
	terraform workspace new california || terraform workspace select california
	terraform init
	terraform apply --var-file regions/california.tfvars --auto-approve

apply-all: virginia oregon california

destroy-virginia: 
	terraform workspace new virginia || terraform workspace select virginia
	terraform init
	terraform destroy --var-file regions/virginia.tfvars --auto-approve

destroy-oregon: 
	terraform workspace new oregon || terraform workspace select oregon
	terraform init
	terraform destroy --var-file regions/oregon.tfvars --auto-approve

destroy-california: 
	terraform workspace new california || terraform workspace select california
	terraform init
	terraform destroy --var-file regions/california.tfvars --auto-approve

destroy-all: destroy-virginia destroy-oregon destroy-california