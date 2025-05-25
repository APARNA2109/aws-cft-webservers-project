# 🪟 Windows Server 2022 EC2 with IIS Deployment via CloudFormation (Across Regions)

## ✅ Project Objective

Deploy a Windows Server 2022 EC2 instance with IIS installed using PowerShell through UserData in AWS CloudFormation in two different regions and verify output through the browser and screenshots.

---

## 🛠️ Step 1: CloudFormation Stack Creation – Region 1

### Description:
Initiated a CloudFormation stack in Region 1 (e.g., N. Virginia). The stack includes an EC2 instance, a security group allowing HTTP access, and other configurations.

### Screenshot:
<div align="center">
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day2-Windows/screenshots/Stack%20creation%20of%20windoeserver(Region1).png" alt="CloudFormation Stack - Region 1" width="600" />
</div>

---

## 📝 Step 2: Parameters Filled – Region 1

### Description:
Provided essential parameters like `InstanceType`, `KeyName`, `VPC`, and `Subnet` while launching the stack.

### Screenshot:
<div align="center">
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day2-Windows/screenshots/paramete%20filler(r1).png" alt="EC2 Running - Region 1" width="600" />
</div>

---

## ⚙️ Step 3: PowerShell Execution via UserData – Region 1

### Description:
Used PowerShell in the `UserData` section to install IIS and serve the default web page automatically on instance launch.

---

## 🌐 Step 4: Website Verified in Browser – Region 1

### Description:
IIS welcome page was successfully displayed using the Public DNS of the EC2 instance from Region 1.

### Screenshot:
<div align="center">
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day2-Windows/screenshots/webserver%20r1.png" alt="Website Output - Region 1" width="600" />
</div>

---

## 🛠️ Step 5: CloudFormation Stack Creation – Region 2

### Description:
Repeated the deployment process in Region 2 (e.g., Ohio) for cross-region testing.

### Screenshot:
<div align="center">
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day2-Windows/screenshots/Stack%20creation%20of%20windoeserver(Region2).png" alt="CloudFormation Stack - Region 2" width="600" />
</div>

---

## 📝 Step 6: Parameters Filled – Region 2

### Description:
Same parameters were filled while launching the stack in Region 2.

### Screenshot:
<div align="center">
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day2-Windows/screenshots/paramete%20filler(r2).png" alt="EC2 Running - Region 2" width="600" />
</div>

---

## ⚙️ Step 7: PowerShell Execution via UserData – Region 2

### Description:
IIS installation was handled in Region 2 using PowerShell inside the CloudFormation UserData script.

---

## 🌐 Step 8: Website Verified in Browser – Region 2

### Description:
Successfully verified the IIS default page in the browser using Public DNS of Region 2 instance.

### Screenshot:
<div align="center">
  <img src="https://github.com/APARNA2109/aws-cft-webservers-project/blob/main/Day2-Windows/screenshots/webserver%20r2.png" alt="Website Output - Region 2" width="600" />
</div>

---

## ✅ Conclusion

Successfully deployed Windows Server 2022 EC2 instances with IIS in **two AWS regions** using CloudFormation and verified the deployment through browser-based output.
