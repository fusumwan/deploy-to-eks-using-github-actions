# deploy-to-eks-using-github-actions
1. Create an EKS Cluster using this command:

Run the aws cloudformation delete-stack Command:

Use the following command to delete the stack:

aws cloudformation delete-stack --stack-name eksctl-primuslearning-cluster --region ap-southeast-2

Monitor the Deletion Process:

You can check the status of the stack deletion with the following command:

aws cloudformation describe-stacks --stack-name eksctl-primuslearning-cluster --region ap-southeast-2




eksctl delete cluster --region=ap-southeast-2 --name=primuslearning

eksctl create cluster --name primuslearning --region ap-southeast-2 --nodegroup-name linux-nodes --node-type t2.micro --nodes 2

2. Then create .github folder and then create workflow folder inside .github folder 
3. create file with .yml extension and write the workflow code
4. Create a github repository 
5. Create secrets in github repo
        Go to settings of repo
        click on secrets and variables
6. Test application by getting the dns name and going to a web browser

Clean up: Run: eksctl delete cluster --name primuslearning
