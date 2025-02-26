#  POC on Dynamic Application Security Testing (DAST) for Java Application


## **Table of Contents**
1. Introduction  
2. Pre-requisites  
3. Step-by-Step Setup Guide  
   - Step 1: Update Your Linux System  
   - Step 2: Install OWASP ZAP  
   - Step 3: Launch OWASP ZAP  
   - Step 4: Perform an Automated Scan  
   - Step 5: Analyze Results  
   - Step 6: Generate Report  
4. Conclusion  
5. Contact Information  
6. References  

## Introduction
This Proof of Concept (POC) aims to demonstrate the effectiveness of DAST in identifying security vulnerabilities in Java applications. 
Dynamic Application Security Testing (DAST) involves evaluating a live application for security vulnerabilities by emulating external threats. OWASP ZAP (Zed Attack Proxy) is a widely used open-source DAST tool designed to detect security flaws in web applications.

## Pre-requisites
- [OWASP ZAP](https://www.zaproxy.org/) 
- **A Running Java Application** to perform DAST.


# Step-by-Step Setup Guide

### **Step 1**: **Update Your Linux System**

- Before installing OWASP ZAP, update your system to ensure you have the latest packages and security patches. Open the terminal and run the following command:

``` bash
sudo apt update
```
### **Step 2: Install OWASP ZAP**

- Once your system is up to date, you can install OWASP ZAP. To do so, type the following command in the terminal:
``` bash
sudo snap install zaproxy --classic
````
![Screenshot 2025-02-26 190125](https://github.com/user-attachments/assets/7df0b26f-d93c-4423-a851-c998c607c050)

### **Step 3: Launch OWASP ZAP**

- Once the installation is complete, you can launch OWASP ZAP from the application menu or the command line. To launch it from the command line, type the following command:
  
``` bash
zaproxy
```
![WhatsApp Image 2025-02-26 at 18 08 40_d4159999](https://github.com/user-attachments/assets/a03f8ae4-682f-48d0-9e35-e5795c0141e6)
- You can now start using OWASP ZAP to test the security of your web applications.After a few minutes, OWASP ZAP will open up.


**Ensure that your application or api should be running before using this service.**
![image](https://github.com/user-attachments/assets/2a787b5e-b147-4ffc-9d63-8195abc3a94e)




### **Step 4: Click on the **Automated scan** option a interface will come out on which provide the URL of the application and click on **attack****


![WhatsApp Image 2025-02-26 at 18 15 27_6453a764](https://github.com/user-attachments/assets/db51b160-3e15-4e1e-86cc-6d61c3672536)

OWASP ZAP will start  scanning  your application for  vulnerabilities .



 ### **Step 5 : Report Generation:** 

You can also Generate the Report of the analysis by click on the **Report** option and generate it in desired format (HTML, PDF,JSON etc.) for future References. 


![WhatsApp Image 2025-02-26 at 18 17 27_1c933a21](https://github.com/user-attachments/assets/8343d0e7-7ee8-4fae-91ff-6b3ec3a347b3)

After selecting the format,click on **Generate Report**. Your Report will be generated in your desired directory. 
![WhatsApp Image 2025-02-26 at 18 18 00_7175835e](https://github.com/user-attachments/assets/c08cb221-e066-48d9-9fd7-1b90898dbe91)

### **Step 6: Report**
| **Link** | **Description** |
|---------|----------------|
| [Download Report](https://github.com/user-attachments/assets/JAVA_DAST_Report.pdf) | Click here to download the generated security analysis report. |


## Conclusion

Dynamic Application Security Testing (DAST) is a crucial method for identifying security vulnerabilities in live applications by simulating real-world attacks. OWASP ZAP, as a leading open-source DAST tool, plays a vital role in uncovering and addressing security issues in web applications, thereby enhancing their resilience against potential threats. By integrating DAST tools like OWASP ZAP into the security testing process, organizations can proactively protect their applications and ensure a robust security posture.

## **Contact Information**


| **Name** | **Email address**            | **Github ID**
|----------|-------------------------------|-------------------|
| Nikita joshi    | Nikita.Joshi@mygurukulam.co    | https://github.com/jnikita19  |

---

## Reference Links

| Links | Description |
|-------|-------------|
|https://techofide.com/blogs/how-to-install-owasp-zap-on-windows-and-linux/ | A step-by-step guide to installing OWASP ZAP on both Windows and Linux platforms. Useful for beginners starting with OWASP ZAP. |
| https://www.zaproxy.org/ | The official website for OWASP ZAP, providing documentation, downloads, and community support. Ideal for exploring all features of ZAP. |
