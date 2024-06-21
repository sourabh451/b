# Ultimate Continuous Integration and Delivery <br> Using Jenkins Pipeline for Spring Boot Java Application <br> with Maven, SonarQube, Argo CD, and Kubernetes

### Watch the Complete Project YouTube Video -> https://www.youtube.com/watch?v=zZfhAXfBvVA&list=RDCMUCnnQ3ybuyFdzvgv2Ky5jnAA&index=1

![Ultimate CI-CD Pipeline Workflow](https://github.com/sourabh451/b/assets/134592493/156009d0-3d24-4310-9527-4441f6b197e6)

![Jenkins Architecture](https://github.com/sourabh451/b/assets/134592493/67d7ca72-38d0-4f2a-863a-18ce72736e99)

### Here are the step-by-step details followed in the above video to set up an Ultimate Continuous Integration and Continuous Delivery process using a Declarative Jenkins pipeline. This pipeline automates the entire CI/CD process for a Spring Boot Java application, starting from the introduction of the workflow, followed by building the application, to production deployment. It uses popular tools like Maven, SonarQube, Docker, Argo CD, and Kubernetes:
```
1. Introduction:
   1.1 Introduction of complete CI/CD pipeline workflow
   1.2 Introduction of Jenkins Architecture

2. Building the simple spring boot java application using maven.

3. Build the Docker images which contains installation and configuration of maven and docker and Push it to the docker registry.

4. Add a Jenkinsfile and Dockerfile to the local repository of spring boot java application to define the pipeline stages.
   4.1 Define the declarative jenkins CI pipeline stages:
        Stage 1: Checkout the source code from Git.
        Stage 2: Build the Java application using Maven.
        Stage 3: Run SonarQube analysis to check the code quality.
        Stage 4: Package the application into a JAR file.
       Build a Dockerfile which copys the jar file from target directory and execute the jar file
        Stage 5: Build and Push Docker Image of our application
        Stage 6: Trigger the CD pipeline using jenkins REST_API

5. Building the Application Manifest for kubernetes configuration:
   5.1 Creating deployment.yml file
   5.2 Creating Jenkinsfile to update the deployment.yml file
   5.3 Creating service.yml file

6. Pushing the Source Code and Application Manifest to Github in two different repositaries

7. Creating Amazon Elastic Compute Cloud i.e EC2 Instance in Amazon Web Service for running jenkins server, sonarqube server and install docker.
   7.1 Install jenkins in EC2 instance for jenkins server
   7.2 Install the necessary Jenkins plugins in jenkins server:
       1.1 Git plugin
       1.2 Maven Integration plugin
       1.3 Pipeline plugin
       1.4 Kubernetes Continuous Deploy plugin

2. Create a new Jenkins pipeline:
   2.1 In Jenkins, create a new pipeline job and configure it with the Git repository URL for the Java application.
   2.2 Add a Jenkinsfile to the Git repository to define the pipeline stages.

3. Define the pipeline stages:
    Stage 1: Checkout the source code from Git.
    Stage 2: Build the Java application using Maven.
    Stage 3: Run unit tests using JUnit and Mockito.
    Stage 4: Run SonarQube analysis to check the code quality.
    Stage 5: Package the application into a JAR file.
    Stage 6: Deploy the application to a test environment using Helm.
    Stage 7: Run user acceptance tests on the deployed application.
    Stage 8: Promote the application to a production environment using Argo CD.

4. Configure Jenkins pipeline stages:
    Stage 1: Use the Git plugin to check out the source code from the Git repository.
    Stage 2: Use the Maven Integration plugin to build the Java application.
    Stage 3: Use the JUnit and Mockito plugins to run unit tests.
    Stage 4: Use the SonarQube plugin to analyze the code quality of the Java application.
    Stage 5: Use the Maven Integration plugin to package the application into a JAR file.
    Stage 6: Use the Kubernetes Continuous Deploy plugin to deploy the application to a test environment using Helm.
    Stage 7: Use a testing framework like Selenium to run user acceptance tests on the deployed application.
    Stage 8: Use Argo CD to promote the application to a production environment.

5. Set up Argo CD:
    Install Argo CD on the Kubernetes cluster.
    Set up a Git repository for Argo CD to track the changes in the Helm charts and Kubernetes manifests.
    Create a Helm chart for the Java application that includes the Kubernetes manifests and Helm values.
    Add the Helm chart to the Git repository that Argo CD is tracking.

6. Configure Jenkins pipeline to integrate with Argo CD:
   6.1 Add the Argo CD API token to Jenkins credentials.
   6.2 Update the Jenkins pipeline to include the Argo CD deployment stage.

7. Run the Jenkins pipeline:
   7.1 Trigger the Jenkins pipeline to start the CI/CD process for the Java application.
   7.2 Monitor the pipeline stages and fix any issues that arise.
```
