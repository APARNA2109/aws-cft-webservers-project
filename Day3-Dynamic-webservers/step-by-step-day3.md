<h1 align="center">🚀 Dynamic Deployment of Windows/Linux Web Servers Using AWS CloudFormation</h1>

---

## 📌 Objective

To build a single AWS CloudFormation Template (CFT) that:

- Accepts user input to choose **Windows**, **Linux**, or **Both**
- Provisions EC2 instances dynamically based on the input
- Installs IIS (Windows) or Apache (Linux) using **User Data scripts**
- Hosts a sample webpage from a public HTML template
- Supports deployment in both **us-east-1** and **us-east-2**

---

## 📋 Requirements

- OS Selection Parameter: Windows / Linux / Both
- Instance Type Parameter (e.g., `t2.micro`)
- SSH Key Pair Name
- Default VPC Usage
- Public HTML Template Download
- No custom AMIs (everything via user data)

---

## 📈 Architecture Flow Chart

<p align="center">
  <img src="images/architecture-diagram.png" alt="Architecture Diagram" width="600"/>
</p>

---

## 📘 Step-by-Step Execution

### 1. AWS Homepage

<p align="center">
  <img src="images/aws-home.png" alt="AWS Homepage" width="700"/>
</p>

---

### 2. Login Page

<p align="center">
  <img src="images/aws-login.png" alt="AWS Login" width="700"/>
</p>

---

### 3. AWS Console

<p align="center">
  <img src="images/aws-console.png" alt="AWS Console" width="700"/>
</p>

---

### 4. Upload CloudFormation Template

- Use: `Day3-Dynamic-webservers.yaml`

<p align="center">
  <img src="images/template-upload.png" alt="CFT Upload" width="700"/>
</p>

---

### 5. Choose AMI (OS Logic Step)

- User selects one: Windows / Linux / Both
- Conditional resources created in CFT

---

### 6. Create Key Pair

- Go to **EC2 > Key Pairs > Create Key Pair**
- Select `.pem` format
- Save securely

*(No screenshot needed)*

---

### 7. Search for CloudFormation

<p align="center">
  <img src="images/cloudformation-search.png" alt="CloudFormation Search" width="700"/>
</p>

---

### 8. Open CloudFormation Console

<p align="center">
  <img src="images/cloudformation-console.png" alt="CloudFormation Console" width="700"/>
</p>

---

### 9. Stack Creation (Where to Click)

<p align="center">
  <img src="images/create-stack-start.png" alt="Create Stack" width="700"/>
</p>

---

### 10. Create Stack from Template

<p align="center">
  <img src="images/create-stack-template.png" alt="Upload Template" width="700"/>
</p>

---

### 11. Specify Stack Details

<p align="center">
  <img src="images/stack-details.png" alt="Stack Details" width="700"/>
</p>

---

### 12. Configure Stack Options

<p align="center">
  <img src="images/configure-options.png" alt="Configure Stack Options" width="700"/>
</p>

---

### 13. Review and Create Stack

<p align="center">
  <img src="images/review-create.png" alt="Review and Create" width="700"/>
</p>

---

### 14. Stack Created Successfully

<p align="center">
  <img src="images/stack-complete.png" alt="Stack Created" width="700"/>
</p>

---

### 15. EC2 Search Page

<p align="center">
  <img src="images/ec2-search.png" alt="EC2 Search" width="700"/>
</p>

---

### 16. EC2 Dashboard

<p align="center">
  <img src="images/ec2-dashboard.png" alt="EC2 Dashboard" width="700"/>
</p>

---

### 17. Linux Instance Running

<p align="center">
  <img src="images/linux-instance.png" alt="Linux Instance" width="700"/>
</p>

---

### 18. Linux Web Server Page

<p align="center">
  <img src="images/linux-webpage.png" alt="Linux Webpage" width="700"/>
</p>

---

### 19. Windows Instance Running

<p align="center">
  <img src="images/windows-instance.png" alt="Windows Instance" width="700"/>
</p>

---

### 20. Windows Web Server Page

<p align="center">
  <img src="images/windows-webpage.png" alt="Windows Webpage" width="700"/>
</p>

---

## 🌎 Repeat for Region: us-east-2

- Follow the exact same steps after switching region in the AWS Console.

---

## ⚠️ Challenges Faced

- Initially, did **not specify `t3` instance type** for Windows — template failed  
- Encountered error “**This site can’t be reached**” using public IP  
  ➤ Fixed by manually typing `http://<public-ip>` instead of just `<public-ip>`  
- Debugging CloudFormation stack events helped understand which condition/resource failed

---

## 🔍 References

- [AWS CloudFormation Docs](https://docs.aws.amazon.com/cloudformation/)
- [Sample HTML Template](https://html5up.net)
- [User Data Scripts](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/user-data.html)
- Personal testing and troubleshooting

---

<h3 align="center">✅ Project Complete! Live web servers running on AWS, fully automated via CloudFormation.</h3>
