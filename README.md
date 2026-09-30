# MARVEL Level 1

This is my Level 1 journey in **Cloud Computing (CL)** and **Cybersecurity (CY)**. It includes the implementation, execution results, outcomes, and key learnings from each task.

---

# CL – Cloud Computing

## Task 1: Working with Git and GitHub Basics

### Overview
This task introduced version control using Git and GitHub and demonstrated how Git is used for collaborative software development.

### Implementation
I practiced cloning repositories, making changes, committing and pushing them to GitHub. I created branches and pull requests and learned how to review and merge changes. I also practiced resolving merge conflicts using rebase and explored `git revert`, `git cherry-pick`, and Git configuration.

### Execution & Results

**Git Repository and Commits**

> Add image here

**Branching and Pull Request**

> Add image here

**Merge Conflict and Rebase**

> Add image here

**Open Source Contribution**

> Add image here

### Outcome
Successfully understood the Git/GitHub development workflow and performed common version-control operations used in collaborative projects.

### Key Learnings
- Version control and distributed repositories
- Git commits and branches
- Pull requests and merging
- Merge conflict resolution
- Git rebase
- Git revert and cherry-pick
- Git configuration
- Open-source contribution workflow

---

## Task 2: Exploring Docker Fundamentals

### Overview
This task introduced Docker, containers, images, and the differences between containers and virtual machines.

### Implementation
I used Docker CLI to pull images from Docker Hub and create containers. I practiced viewing running containers, checking logs, inspecting containers, and managing their complete lifecycle.

### Execution & Results

**Docker Image Pull**

> Add image here

**Running Container**

> Add image here

**Docker Container in Browser**

> Add image here

### Outcome
Successfully created and managed Docker containers and understood how containers provide lightweight application environments.

### Key Learnings
- Containers vs Virtual Machines
- Docker images and containers
- Docker Hub
- Docker CLI
- Container logs and inspection
- Start, stop, restart and remove containers

---

## Task 3: Dockerize a Simple Application

### Overview
This task focused on packaging a simple application into a Docker container using a Dockerfile.

### Implementation
I created a simple application and wrote a Dockerfile containing the required instructions. I built a Docker image, started a container, mapped the required ports, and accessed the application from the browser.

### Execution & Results

**Dockerfile**

> Add image here

**Docker Image Build**

> Add image here

**Application Running in Container**

> Add image here

### Outcome
Successfully containerized an application and accessed it locally through a Docker container.

### Key Learnings
- Dockerfile structure
- Building Docker images
- Running containers
- Port mapping
- Docker image layers
- Containerizing applications

---

## Task 4: Launch and Manage an AWS EC2 Instance

### Overview
This task introduced AWS EC2 and demonstrated how virtual machines can be created and managed in the cloud.

### Implementation
I launched an EC2 instance and configured its security group for SSH and HTTP traffic. I connected to the instance using SSH with a `.pem` key and installed the Nginx web server. I then accessed Nginx using the EC2 public IP.

### Execution & Results

**EC2 Instance Running**

> Add image here

**SSH Connection**

> Add image here

**Nginx Installation**

> Add image here

**Nginx through Public IP**

> Add image here

### Outcome
Successfully launched and remotely managed an AWS EC2 virtual machine and hosted a web server on it.

### Key Learnings
- AWS EC2
- Cloud virtual machines
- EC2 instance types
- Security groups
- SSH
- Public IP addresses
- Nginx web server
- CPU and memory allocation

---

## Task 5: Kubernetes Basics and Writing Pod Specs

### Overview
This task introduced Kubernetes architecture and basic resources such as clusters, nodes, pods, and the control plane.

### Implementation
I created a local Kubernetes cluster using Minikube. I wrote a YAML manifest to create an Nginx Pod and deployed it using `kubectl`. I also inspected the Pod status, description, and logs.

### Execution & Results

**Minikube Cluster**

> Add image here

**Pod Deployment**

> Add image here

**Pod Status and Details**

> Add image here

### Outcome
Successfully created and managed a Kubernetes Pod using YAML manifests and `kubectl`.

### Key Learnings
- Kubernetes clusters
- Nodes
- Pods
- Control Plane
- YAML manifests
- Minikube
- kubectl
- Pod status and logs

---

## Task 6: Manage AWS S3 and IAM with CLI

### Overview
This task introduced AWS Identity and Access Management (IAM), S3 cloud storage, and AWS CLI.

### Implementation
I created an IAM user with the required permissions and configured AWS CLI. Using CLI commands, I created an S3 bucket and performed file upload, listing, download, and deletion operations.

### Execution & Results

**IAM User and Permissions**

> Add image here

**AWS CLI Configuration**

> Add image here

**S3 Bucket Creation**

> Add image here

**File Upload and S3 Operations**

> Add image here

### Outcome
Successfully managed AWS S3 resources through the command line using IAM-based authentication and permissions.

### Key Learnings
- IAM users
- IAM roles and policies
- Least-privilege principle
- AWS CLI
- S3 buckets
- S3 objects
- Uploading and downloading files

---

## Task 7: Deploy a Containerized Application on Kubernetes

### Overview
This task focused on deploying and managing a containerized application using Kubernetes Deployments and Services.

### Implementation
I created a Deployment YAML for my Dockerized application and deployed multiple replicas. I used ClusterIP for internal access and NodePort for external access. I also practiced scaling the deployment and observing application updates.

### Execution & Results

**Kubernetes Deployment**

> Add image here

**Multiple Running Pods**

> Add image here

**ClusterIP and NodePort Services**

> Add image here

**Application Running through NodePort**

> Add image here

### Outcome
Successfully deployed, exposed, and scaled a containerized application using Kubernetes.

### Key Learnings
- Kubernetes Deployments
- Replica management
- ClusterIP
- NodePort
- Kubernetes Services
- Application scaling
- Rolling updates

---

## Task 8: Use Kubernetes Secrets and Environment Variables

### Overview
This task focused on securely managing application configuration and sensitive information inside Kubernetes.

### Implementation
I created a ConfigMap for normal application configuration and a Kubernetes Secret for AWS credentials. I updated the Deployment to inject these values into the container through environment variables.

### Execution & Results

**ConfigMap Creation**

> Add image here

**Kubernetes Secret Creation**

> Add image here

**Deployment with Environment Variables**

> Add image here

**Application Interaction with AWS**

> Add image here

### Outcome
Successfully separated application configuration and sensitive credentials from the application source code.

### Key Learnings
- Kubernetes ConfigMaps
- Kubernetes Secrets
- Environment variables
- Secret management
- Secure credential handling
- Difference between Secrets and ConfigMaps

---

## Task 9: Deploy an App to Push Files from Kubernetes to S3

### Overview
This task combined the concepts learned throughout the Cloud Computing module into one complete application.

The goal was to deploy an application on Kubernetes that could upload files directly to an AWS S3 bucket.

### Implementation
I developed a file-upload application and containerized it using Docker. The Docker image was deployed to Minikube using Kubernetes.

AWS credentials were stored using Kubernetes Secrets and injected into the application as environment variables. The application used these credentials to communicate with AWS S3 and upload files.

The complete workflow was:

**User → Application → Docker → Kubernetes → Kubernetes Secrets → AWS S3**

### Execution & Results

**Docker Image Build**

> Add image here

**Kubernetes Deployment**

> Add image here

**Running Application**

> Add image here

**File Selection and Upload**

> Add image here

**Successful Upload**

> Add image here

**Uploaded File in AWS S3**

> Add image here

### Outcome
Successfully developed and deployed a complete application that uploads files from a Kubernetes-hosted application to AWS S3.

This task successfully integrated Docker, Kubernetes, IAM, S3, ConfigMaps, and Secrets into a single working pipeline.

### Key Learnings
- Building a complete cloud application
- Docker containerization
- Kubernetes deployment
- Kubernetes Services
- Kubernetes Secrets
- AWS IAM authentication
- AWS S3 integration
- Application-to-cloud communication
- Integration of multiple DevOps and cloud technologies

---

# CY – Cybersecurity

## Level 1: Cybersecurity Fundamentals

### Overview
The Cybersecurity Level 1 module focused on building the fundamental knowledge required to understand cybersecurity.

The module covered networking, protocols, Windows, Linux, and core cybersecurity principles through practical exercises on TryHackMe.

### Implementation
I created a TryHackMe account and accessed the MARVEL Level 1 Cybersecurity module. I completed the provided learning sections, practical exercises, and challenges.

The module helped me understand how computers communicate over networks and how operating systems and security mechanisms work.

### Execution & Results

**TryHackMe MARVEL Module**

> Add image here

**Networking Fundamentals**

> Add image here

**Protocols and Networking Tasks**

> Add image here

**Windows Fundamentals**

> Add image here

**Linux Fundamentals**

> Add image here

**Cybersecurity Fundamentals**

> Add image here

**Completed Tasks**

> Add image here

### Outcome
Successfully completed the Level 1 cybersecurity fundamentals and gained a stronger understanding of networking, operating systems, protocols, and basic security concepts.

### Key Learnings
- Computer networking fundamentals
- IP and MAC addresses
- Ports
- TCP and UDP
- DNS and DHCP
- Common networking protocols
- Windows fundamentals
- Linux fundamentals
- CIA Triad
- Vulnerabilities
- Offensive security basics
- Defensive security basics
- Importance of authorization and scope in security testing

---

# Overall Outcome

MARVEL Level 1 provided practical exposure to two important technical domains: **Cloud Computing and Cybersecurity**.

In Cloud Computing, I learned how applications can move through the complete workflow:

**GitHub → Docker → Kubernetes → AWS**

I gained hands-on experience with Git, Docker, AWS EC2, IAM, S3, Kubernetes, Minikube, ConfigMaps, and Secrets.

In Cybersecurity, I developed a stronger foundation in networking, protocols, Windows, Linux, and security principles through TryHackMe exercises.

---

# Overall Key Learnings

Through Level 1, I gained practical experience in:

- Version control and collaborative development
- Containerization
- Cloud virtual machines
- Cloud storage
- Identity and access management
- Container orchestration
- Application deployment
- Configuration and secret management
- Networking fundamentals
- Operating system fundamentals
- Cybersecurity fundamentals
- Offensive and defensive security concepts

These tasks provided a strong foundation for progressing into more advanced **Cloud, DevOps, and Cybersecurity** concepts.