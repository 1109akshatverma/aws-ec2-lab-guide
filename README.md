# Lab Guide: Launching an EC2 Instance on AWS

## Prerequisites

Before starting this lab, make sure you have:

- An active AWS account
- IAM user with permission to launch EC2 instances

---

##  Step 1: Login to AWS Management Console

1. Go to [https://aws.amazon.com/](https://aws.amazon.com/)
2. Click **Sign In to the Console**
3. Use your **IAM credentials** or **root user** login

<img src="./Images/3. A.png" width="950" alt="Log in to AWS console with credentials"/>

---

##  Step 2: Navigate to EC2 Dashboard

1. In the **search bar**, type **EC2**
2. Select **EC2** under “Services”
3. You will be directed to the EC2 Dashboard

---

##  Step 3: Launch a New Instance

1. Click **Launch Instance**
2. Provide a name, e.g., `ak-ec2`


#### A. Choose Amazon Machine Image (AMI)

- Select **Amazon Linux 2023 AMI (Free Tier eligible)**

#### B. Choose Instance Type

- Select **t2.micro** (Free Tier eligible)

#### C. Key Pair (Login)

1. Choose an existing key pair or
2. Create a new one
   - Download and save the `.pem` file securely

#### D. Configure Security Group

- Allow **SSH** access (port 22) from your IP to connect to your EC2

#### E. Configure Storage

- Default settings (8 GB) are fine for most use cases

#### F. Review and Launch

1. Click **Launch Instance**
2. Wait for instance status to become **Running**

---

##  Step 4: Connect to Your EC2 Instance

1. Select your instance in the EC2 Dashboard
2. Click **Connect**
3. Choose **SSH client**
4. Follow the connection instructions (sample below):
5. Open **Terminal** in your windows and navigate to your key (ak-key.pem)
6. Paste the following commands on terminal


