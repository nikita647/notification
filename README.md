

# **POC for Slack and Email Notifications in Jenkins**


## **Table of Contents**  
1. [Introduction](#introduction)  
2. [Prerequisites](#prerequisites)  
3. [Step-by-Step Setup](#step-by-step-setup)  
   - [Step 1: Create a Slack Account](#step-1-create-a-slack-account)  
   - [Step 2: Install Jenkins CI App on Slack](#step-2-install-jenkins-ci-app-on-slack)  
   - [Step 3: Install Slack Plugin in Jenkins](#step-3-install-slack-plugin-in-jenkins)  
   
   - [Step 4: Run a Sample Test](#step-4-run-a-sample-test)  



## **Introduction**

This guide explains how to set up Slack notifications in Jenkins. By integrating Slack with Jenkins, you can receive real-time updates about your builds, making it easier for your team to stay informed and act quickly.


## **Prerequisites**

- **Slack Account:** You need a Slack workspace and a channel where Jenkins can send notifications.
- **Jenkins Server:** A Jenkins server up and running.
- **Slack Plugin:** The Slack Notification Plugin must be installed in Jenkins.


## **Step-by-Step Setup**

###  **Step 1: Create a Slack Account**

1. Go to [Slack’s official website](https://slack.com) and click **Sign Up**.

2.  Create a workspace (e.g., "Jenkins").

3.  Set up a Slack channel for notifications.
   
![image](https://github.com/user-attachments/assets/3ab51982-f91f-41a9-aa26-22851b760380)

### **Step 2: Install Jenkins CI App on Slack**

1. Open Slack and go to Settings & Administration > Manage Apps.

2. Search for Jenkins CI and click Add to Slack.

3. Choose a Slack channel for Jenkins notifications.
   
![image](https://github.com/user-attachments/assets/c06ad9e3-fcc9-4784-ad0c-be947e4685e2)

![image](https://github.com/user-attachments/assets/629764cc-d288-4692-a2ba-4888b9688ae3)

![image](https://github.com/user-attachments/assets/b66ac361-89f6-4398-b669-46136666bd9c)


**4. Choose the Slack channel where you want to receive Jenkins notifications, then click **Add Jenkins CI Integration****

![image](https://github.com/user-attachments/assets/65e770dd-d758-4f42-877b-5c8f685f8d36)


**5. Copy the **team subdomain** and **integration token** for later use in Jenkins.****

![image](https://github.com/user-attachments/assets/e94237ff-a9b1-40dd-9559-1f8db21203a6)



### **Step 3. Install Slack Plugin in Jenkins**

1. Install the Plugin:

2. Go to your Jenkins dashboard.

3. Navigate to Manage Jenkins > Manage Plugins.

4. Search for "Slack Notification Plugin" and install it.

![image](https://github.com/user-attachments/assets/e0f5a5ba-6df2-4fa1-9f60-4251132ff2bb)


5. **configure the Slack credentials:**

- Go to Manage Jenkins > Credentials > Global > Add Credentials.
- Select Secret Text, then enter the Slack integration token copied earlier.



![image](https://github.com/user-attachments/assets/58babd05-dc51-46de-83fd-cf49aca62db7)

![image](https://github.com/user-attachments/assets/282bed9d-b2da-4c93-829c-d5338102f77c)


6. **Configure the Slack settings in Jenkins:**

- Go to Manage Jenkins > Configure System.
- In the Slack section:

   - Set Workspace to your Slack team subdomain.
   - Select the credentials (integration token) you created earlier.
   - Set a default Slack channel for notifications.

![image](https://github.com/user-attachments/assets/8a4ad68c-83d9-4f36-8601-eea94b6a41e6)

![image](https://github.com/user-attachments/assets/dc8469d4-9cc3-484e-afb8-24797e48f285)


### **Step 4: Run a Sample Test**
1. Trigger a build

2. Check the Slack channel you configured to ensure you receive build status notifications.



![image](https://github.com/user-attachments/assets/228a0393-7211-4ffb-bc0a-caa2d9318185)


