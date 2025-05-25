# Apache Web Server Deployment using AWS CloudFormation (Across Regions)

## ✅ Project Objective

Deploy an Apache web server on an EC2 instance using AWS CloudFormation in two different regions and verify it through browser and screenshots.

---

## 🛠️ Step 1: CloudFormation Stack Creation – Region 1

### Description:
We initiated a CloudFormation stack in Region 1 (e.g., N. Virginia). The stack includes EC2, security group, and required configurations.

### Screenshot:
<div>
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day1-Linux/screenshots/Stack%20creation%20of%20linuxserver(Region1).png" alt="CloudFormation Stack - Region 1" width="600" />
</div>

---

## 📝 Step 2: Parameters Filled – Region 1

### Description:
While launching the CloudFormation stack, parameters like InstanceType, KeyName, and SSHLocation were provided.

### Screenshot:
<div>
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day1-Linux/screenshots/parametersfilled%20(region%201).png" alt="Parameters Filled - Region 1" width="600" />
</div>

---

## 🖥️ Step 3: EC2 Instance Running – Region 1

### Description:
The EC2 instance created by the stack is now in the running state.

### Screenshot:
<div>
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day1-Linux/screenshots/ec2%20running(region%201).png" alt="EC2 Instance - Region 1" width="600" />
</div>

---

## 🌐 Step 4: Website Verified in Browser – Region 1

### Description:
The Apache web server shows a welcome page when accessed through the public IP or DNS.

### Screenshot:
<div>
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day1-Linux/screenshots/web%20server%20(region1).png" alt="Browser Output - Region 1" width="600" />
</div>

---

## 🌎 Step 5: CloudFormation Stack Creation – Region 2

### Description:
We repeated the process in Region 2 (e.g., Ohio) to test cross-region setup.

### Screenshot:
<div>
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day1-Linux/screenshots/Stack%20creation%20of%20linuxserver(Region2).png" alt="CloudFormation Stack - Region 2" width="600" />
</div>

---

## 📝 Step 6: Parameters Filled – Region 2

### Description:
Entered the same parameters used for Region 1.

### Screenshot:
<div>
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day1-Linux/screenshots/parametersfilled%20(region%202).png" alt="Parameters Filled - Region 2" width="600" />
</div>

---

## 🖥️ Step 7: EC2 Instance Running – Region 2

### Description:
The EC2 instance in Region 2 is up and running.

### Screenshot:
<div>
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day1-Linux/screenshots/ec2%20running(region%202).png" alt="EC2 Instance - Region 2" width="600" />
</div>

---

## 🌐 Step 8: Website Verified in Browser – Region 2

### Description:
Verified the public IP and DNS from Region 2 also display the Apache welcome page.

### Screenshot:
<div>
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day1-Linux/screenshots/web%20server%20(region2).png" alt="Browser Output - Region 2" width="600" />
</div>

---

## ✅ Conclusion

Successfully deployed and verified Apache Web Server in two AWS regions using CloudFormation.
