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

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/1.%20Login%20to%20AWS%20Management%20Console.png?raw=true" width="950" />


---

##  Step 2: Navigate to EC2 Dashboard

1. In the **search bar**, type **EC2**
2. Select **EC2** under “Services”
3. You will be directed to the EC2 Dashboard

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/2.%20Navigate%20to%20EC2%20Dashboard.png?raw=true" width="950" />
---

##  Step 3: Launch a New Instance

1. Click **Launch Instance**
2. Provide a name, e.g., `ak-ec2`

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/3.%20Launch%20a%20New%20Instance.png?raw=true" width="950" />

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/3.%20Name.png?raw=true" width="950" />



#### A. Choose Amazon Machine Image (AMI)

- Select **Amazon Linux 2023 AMI (Free Tier eligible)**

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/3.%20A.png?raw=true" width="950" />

#### B. Choose Instance Type

- Select **t2.micro** (Free Tier eligible)

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/3.%20B.png?raw=true" width="950" />

#### C. Key Pair (Login)

1. Choose an existing key pair or
2. Create a new one
   - Download and save the `.pem` file securely

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/3.%20C1.png?raw=true" width="950" />

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/3.%20C2.png?raw=true" width="950" />

#### D. Configure Security Group

- Allow **SSH** access (port 22) from your IP to connect to your EC2

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/3.%20D.png?raw=true" width="950" />

#### E. Configure Storage

- Default settings (8 GB) are fine for most use cases

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/3.%20E.png?raw=true" width="950" />

#### F. Review and Launch

1. Click **Launch Instance**
2. Wait for instance status to become **Running**

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/3.%20F1.png?raw=true" width="950" />

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/3.%20F2.png?raw=true" width="950" />

---

##  Step 4: Connect to Your EC2 Instance

1. Select your instance in the EC2 Dashboard
2. Click **Connect**
3. Choose **SSH client**
4. Follow the connection instructions (sample below):
5. Open **Terminal** in your windows and navigate to your key (ak-key.pem)
6. Paste the following commands on terminal

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/4.%20Connect.png?raw=true" width="950" />

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/4.%20A.png?raw=true" width="950" />

<img src="https://github.com/1109akshatverma/aws-ec2-lab-guide/blob/main/Images/4.%20B.png?raw=true" width="950" />

---

## AWS EC2 Documentation

You can read the official documentation here:  
[Amazon EC2 User Guide](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html)

---

## Conclusion

You’ve now successfully launched an EC2 instance using the AWS Console. You can repeat this process to launch more instances, connect via SSH, and explore advanced features like Elastic IPs, security groups, or load balancers.