# EC2 Fundamentals

## Step 1: Video Lecture & Core Concepts

Infrastructure as a Service (IaaS) shifts the responsibility of physical hardware management from the company to AWS. AWS manages the physical servers, networking hardware, power, cooling, and maintenance inside their data centers. The customer is responsible for managing the operating system, applications, deployment, and server configuration.

---

# Step 2: Theoretical Analysis

## 1. Why does EC2 stand for "Elastic Compute Cloud"?

Amazon EC2 stands for Elastic Compute Cloud because cloud resources can scale up or down depending on demand. The word elastic refers to the ability to quickly increase or decrease computing resources whenever needed. If traffic increases, more instances can be launched. If demand decreases, instances can be shut down to reduce costs.

---

## 2. Four Essential Infrastructure Features Provided by EC2

### Compute Power
EC2 provides virtual CPUs and memory resources that allow users to run applications and services inside virtual machines.

### Storage
EC2 provides storage options for saving files, applications, databases, and operating system data.

### Networking
EC2 includes networking capabilities such as IP addresses, internet connectivity, ports, and security groups for controlling incoming and outgoing traffic.

### Operating System Control
Users have full control over the operating system and can install software, configure services, and manage deployments on the server.

---

## 3. EC2 Billing Model

EC2 uses a pay-as-you-go billing model. Customers only pay for the computing resources they actively use. When demand decreases and instances are scaled down or shut down, costs are reduced because fewer resources are being consumed.

---

# Step 3: Bootstrapping Design (User Data)

## What is the process of bundling configuration commands into a script called?

The process of bundling configuration commands into a startup script is called bootstrapping.

---

## Under which specific user profile are User Data scripts executed?

User Data scripts are executed under the root user profile, which has administrative privileges on the EC2 instance.

---

## How many times does a User Data script run during the lifecycle of an EC2 instance?

A User Data script normally runs one time during the first boot of the EC2 instance.
