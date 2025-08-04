# Task-1_04-08-2025
Automate Code Deployment Using CI/CD Pipeline (GitHub Actions)
--------------------------------------------------------------

Took a demo Node.js application which simply gives the result "Welcome to DevOps !!".
Node.js application consists of index.js, package.json and Dockerfile in the repository.
github workflow is created.
main.yml file is set to "Trigger on push to main".
build-and-deploy job is configured which do code checkout, install Node.js, dependencies, build docker image and later on pushes the docker image to docker hub.
Secrets are created to login to docker (username and password) repository level which is used in main.yml file.
The created image can be deployed to a remote server like ec2 instance etc.
To deploy the web application we can create secrets like REMOTE_HOST, REMOTE_USER AND SSH_PRIVATE_KEY at repository level similar to what we did while docker login step in main.yml.
