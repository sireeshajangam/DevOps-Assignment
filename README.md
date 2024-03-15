CONTINUOUS INTEGRATION AND DEPLOYMENT:
STEPS:
created a simple pythonapplication with message "azure web apps"
created a Docker file with using alpine for lightweight 
I created a workflow using gitHub Actions,that automatically checkout the code from github and build image and then push to ECR.It includes the Following steps
To maintain the aws credentinals securely , i stored them on github secrets
Finally i craeted a Dockerrun.aws.json file which  includes the path to newly pushed image url.
And then i deployed that file in Elastic Beanstalk with necessary configuraion which includes creation of roles with plocies AmazonEC2ConatinerRegistryAccessPolicy and security groups 
Successfully deployed using Elasic Beanstalk
