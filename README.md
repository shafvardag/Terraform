# Now we can work with the main.tf file in globo_web_app
cd globo_web_app

# Open the main.tf file in your code editor and replace the values 
# for the AWS keys in the config file

# Now we will follow the standard Terraform workflow
terraform init
terraform plan -out m3.tfplan
terraform apply "m3.tfplan"

# Got to the Console and get the Public IP address for the EC2 instance
# and browse to port 80.

# If you are done, you can tear things down to save $$
terraform destroy

