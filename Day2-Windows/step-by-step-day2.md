# ✅ Windows Server 2022 EC2 with IIS Deployment via CloudFormation

## ✅ Project Objective

Deploy a Windows Server 2022 EC2 instance with IIS installed using PowerShell through UserData in a CloudFormation template.

---

## 🛠️ Step 1: CloudFormation Stack Creation

### Description:
Initiated a CloudFormation stack with resources including an EC2 instance, a security group allowing HTTP access, and required configurations.

### Screenshot:
![CloudFormation Stack Creation](screenshots/stack.png)

---

## 📝 Step 2: Parameters Filled

### Description:
Provided essential parameters like `InstanceType`, `KeyName`, `VPC`, and `Subnet` while launching the stack.

### Screenshot:
![EC2 Running](screenshots/ec2.png)

---

## ⚙️ Step 3: PowerShell Execution via UserData

### Description:
Used PowerShell in the `UserData` section to install IIS and serve the default web page. The script was executed automatically on instance launch.

---

## 🌐 Step 4: Website Verified in Browser

### Description:
IIS welcome page was successfully displayed via the Public DNS of the EC2 instance.

### Screenshot:
![Website Output - IIS](screenshots/site.png)

---

## ✅ Conclusion

Successfully deployed a Windows EC2 instance with IIS using AWS CloudFormation and validated the setup via a web browser.
