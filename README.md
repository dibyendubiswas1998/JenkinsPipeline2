# Second Jenkins Pipeline:
Simple Pipeline for Deploying the application on EC2 Instance (inside Jenkins Master Node).<be>
**Note:** Here I use docker-compose concepts to rebuild and rerun and redeploy the application.

## Steps:
* Create the Application,
* Create a Dockerfile,
* Write a Pipeline file **`.jenkins/Jenkinsfile`**
* Get the Credentials from DockerHub, as AccessToken,
* Install the Jenkins,
* Store the DockerHub credentials in the jenkins credentials as **dockerhub** and access as `DOCKERHUB_CREDENTIALS` and `DOCKERHUB_CREDENTIALS_USR` for username and `DOCKERHUB_CREDENTIALS_PSW` as password.
* Create a Job in Jenkins using Pipeline,
* Trigger the Pipeline when Poll SCM (after every minute),
* Mentions URL, branch, **`.jenkins/Jenkinsfile`** into Jenkins Pipeline.
