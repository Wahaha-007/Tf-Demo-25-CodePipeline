# Tf-Demo-25-CodePipeline

1. Remark only : Old version Docker login

   $(aws ecr get-login --no-include-email)

2. To use GIT in Wondows to connect to CodeCommit

Step 3: Edit Local SSH Configuration
Edit your SSH configuration file named config in your local ~/.ssh directory. Add the following lines to the file, where the value for User is the SSH Key ID you copied in Step 2.

Host git-codecommit.\*.amazonaws.com
User Your-IAM-SSH-Key-ID-Here
IdentityFile ~/.ssh/Your-Private-Key-File-Name-Here

3. Use Terraform plan first, it seems like the fresh download of library
   .terraform/modules/vpc/main.tf need some locally mod before real apply

4. The latest code can build succesfully but when deploy will alternating swap between green and blue forever !

   Need to look at deployment related code carefully again
