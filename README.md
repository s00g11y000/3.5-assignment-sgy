# 3.5-assignment-sgy
Steps:
-Create a repository in AWS ECR 

-Run aws configure to configure access keys and secret keys

-Authenticate docker client with aws with: "aws ecr get-login-password --region region | docker login --username AWS --password-stdin aws_account_id.dkr.ecr.region.amazonaws.com"

-Terraform basic config files

-Run docker image build -t <image> .

-Given that us-west-2 is the region, tag your image with aws ecr repository: docker tag "local image ID" aws_account_id.dkr.ecr.us-west-2.amazonaws.com/my-repository:tag

-Do a docker push to the aws ecr repository: docker push aws_account_id.dkr.ecr.us-west-2.amazonaws.com/my-repository:tag