CONTINUOUS INTEGRATION AND DEPLOYMENT:
1.created a simple pythonapplication with message "azure web apps"
2.created a Docker file with using alpine for lightweight 
3.I created a workflow using gitHub Actions,that automatically checkout the code from github and build image and then push to ECR.It includes the Following steps
4.To maintain the aws credentinals securely , i stored them on github secrets
5.Finally i craeted a Dockerrun.aws.json file which  includes the path to newly pushed image url.
6.And then i deployed that file in Elastic Beanstalk with necessary configuraion which includes creation of roles with plocies AmazonEC2ConatinerRegistryAccessPolicy and security groups 
7.Successfully deployed using Elasic Beanstalk
