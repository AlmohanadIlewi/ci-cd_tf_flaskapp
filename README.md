# ci-cd_tf_flaskapp

- Al Mohanad Ilewi@AWSCloud MINGW64 ~/Desktop/Tools/ci-cd_tf_flaskapp (main)
$ terraform -chdir=terraform init

Initializing the backend...
bucket
  The name of the S3 bucket

  Enter a value: cicd-bucket123

  - terraform -chdir=terraform validate
  - terraform -chdir=terraform plan

- $  terraform -chdir=terraform/ output -raw inventory
  [app_servers]
app0 ansible_host="18.153.83.32"
app1 ansible_host="18.197.201.207"

- $  terraform -chdir=terraform/ output dns_name
  "http://web-app-lb-2045459923.eu-central-1.elb.amazonaws.com"