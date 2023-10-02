![image](https://github.com/amit9974/aws-end-to-end-continuous-integration-real-time-project-/assets/88576479/7486c4b0-8a32-48b2-8e36-03b02c667cc7)

# aws-end-to-end-continuous-integration-real-time-project-
🚀 Here's a step-by-step guide to create an end-to-end Continuous Integration (CI) pipeline on AWS using IAM, CodeBuild, CodePipeline, and Docker to build and push 
a Docker image to Docker Hub.

# Set Up AWS IAM Roles 🧑‍💼
![image](https://github.com/amit9974/aws-end-to-end-continuous-integration-real-time-project-/assets/88576479/084d29b3-47bd-4552-99ed-0c37bf9bba82)

Create IAM roles for your services, such as CodeBuildRole and CodePipelineRole, with appropriate permissions.
Attach policies for necessary AWS services like S3, ECR, and CodeBuild.

# Integrate with GitHub
Integrate your project with GitHub for Repository access.

# Push Code to GitHub 📦
Push your code to a source code repository like GitHub.

# Create an AWS CodeBuild Project 🏗️
![image](https://github.com/amit9974/aws-end-to-end-continuous-integration-real-time-project-/assets/88576479/fdb82c72-54e2-4237-8ffc-9d6fb73a7daa)

Configure a CodeBuild project to build your application and create a Docker image.
Specify the Docker image name and tag.

# Set Up DockerHub Account 🐳
Create an account on Docker Hub (if you don't have one).
Create a repository to store your Docker image.
Configure SystemsManager Parameter for storing docker credentials.
![image](https://github.com/amit9974/aws-end-to-end-continuous-integration-real-time-project-/assets/88576479/fe634ffa-68f7-4cb0-9ef8-575fc1b86e70)


# Create an AWS CodePipeline 🚀
Create a CodePipeline to automate the CI/CD process.
Connect your source repository and CodeBuild project.
Add a build stage to trigger CodeBuild.

# Configure AWS CodePipeline Stages ⚙️
![image](https://github.com/amit9974/aws-end-to-end-continuous-integration-real-time-project-/assets/88576479/a9741aab-cd45-4afa-acbf-5146ab638226)

Define stages in your pipeline:
![image](https://github.com/amit9974/aws-end-to-end-continuous-integration-real-time-project-/assets/88576479/cc4d1e67-7fea-4421-aa03-bc8462477f42)

Source: Connect to your code repository.
Build: Use CodeBuild to build the Docker image.
Deploy: Push the Docker image to Docker Hub.
Add Environment Variables 🤖

In CodeBuild, set environment variables for DockerHub credentials.
Ensure that these credentials are securely stored in AWS Secret Manager or SSM Parameter Store.

# Test and Validate Your Pipeline 🧪
Run a test build in CodePipeline to ensure everything works as expected.

# Start Build Project 🧪
Your docker image is start building & now it is sucessfully push on Docker Hub.
![image](https://github.com/amit9974/aws-end-to-end-continuous-integration-real-time-project-/assets/88576479/15c9ca74-f985-403f-98b7-61648076ae5c)

