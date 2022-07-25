### Validating Kubernetes Configurations with Datree
Working with Kubernetes is fun when your Kubernetes cluster is up and your nodes are working as you expected. But as a DevOps enthusiast who follows the principles of Continuous Integration and Continuous Delivery, you are aware that new changes or feature requests are always coming through the Jenkins Pipeline, and eventually, you’ll have to deploy changes into the Kubernetes cluster which feeds into your production environment.

### What is Datree?
Datree allows developers to verify the Kubernetes configuration before applying it directly into the Production, Stage, Test, or even the Development environment. Datree is a command-line tool that is installed locally onto the developer’s machine so that he or she can run the CLI commands that verify the Kubernetes manifests (YAML files).

### Here is a short command snippet of Datree -
datree test my-kubernetes-manifest.yaml

### 1. How to Install Datree?
curl https://get.datree.io | /bin/bash

### 2. How to test Kubernetes Manifest using Datree
datree test <your_kubernetes_manifest_YAML_NAME>

Here is my Kubernetes manifest(YAML) of my Spring Boot application which I am trying to test by deploying it on Kubernetes Cluster

[Click here to clone my GitHub Repo for Spring Boot Application](https://github.com/gayatrisingh31/k8s-springboot/tree/main/src)

### Creating one directory
we will create one directory after we will create one file which name is:
k8s-springboot-deployment.yaml

### Here is a command to test my Kubernetes manifest -

datree test k8s-spring-boot-deployment.yml

### 4. View and edit Datree Policy via browser
This too is pretty simple. Run the test command datree test k8s-spring-boot-deployment.yml and then look for the following message box into your terminal -

![Manifest Placeholders Dashboard](./images/dat1.png "Edit Manifest Placeholders")


![view and edit](./images/dat1.png "datree")
