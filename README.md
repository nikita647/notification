# notification

# **POC for Slack Notifications in Jenkins**

Table of content


## Introduction

This guide explains how to set up Slack notifications in Jenkins. By integrating Slack with Jenkins, you can receive real-time updates about your builds, making it easier for your team to stay informed and act quickly.

## Prerequisites

- **Slack Account:** You need a Slack workspace and a channel where Jenkins can send notifications.
- **Jenkins Server:** A Jenkins server up and running.
- **Slack Plugin:** The Slack Notification Plugin must be installed in Jenkins.


**Step-by-Step Setup**

##  Step 1: Create a Slack Account

1. Go to [Slack’s official website](https://slack.com) and click **Sign Up**.

2. Create a workspace (e.g., "Jenkins").

3. Set up a Slack channel for notifications.
   
![image](https://github.com/user-attachments/assets/3ab51982-f91f-41a9-aa26-22851b760380)

**Step 2: Install Jenkins CI App on Slack**

- Open Slack and go to Settings & Administration > Manage Apps.

- Search for Jenkins CI and click Add to Slack.

- Choose a Slack channel for Jenkins notifications.
   
![image](https://github.com/user-attachments/assets/c06ad9e3-fcc9-4784-ad0c-be947e4685e2)

![image](https://github.com/user-attachments/assets/629764cc-d288-4692-a2ba-4888b9688ae3)

![image](https://github.com/user-attachments/assets/b66ac361-89f6-4398-b669-46136666bd9c)

4. Choose the Slack channel where you want to receive Jenkins notifications, then click **Add Jenkins CI Integration**.

![image](https://github.com/user-attachments/assets/65e770dd-d758-4f42-877b-5c8f685f8d36)

5. Copy the **team subdomain** and **integration token** for later use in Jenkins.

![image](https://github.com/user-attachments/assets/e94237ff-a9b1-40dd-9559-1f8db21203a6)



2. Install Slack Plugin in Jenkins

   Install the Plugin:

Go to your Jenkins dashboard.

Navigate to Manage Jenkins > Manage Plugins.

Search for "Slack Notification Plugin" and install it.


After installation, configure the Slack credentials:

Go to Manage Jenkins > Credentials > Global > Add Credentials.
Select Secret Text, then enter the Slack integration token copied earlier.


Step 4: Run a Sample Test
1.Trigger a build
2.Check the Slack channel you configured to ensure you receive build status notifications.

![image](https://github.com/user-attachments/assets/e0f5a5ba-6df2-4fa1-9f60-4251132ff2bb)

![image](https://github.com/user-attachments/assets/a963c765-916e-47b3-abd8-0efb6054aa34)

![image](https://github.com/user-attachments/assets/739cfba5-5b1d-4573-b6ce-49d5fdfc8906)

![image](https://github.com/user-attachments/assets/58babd05-dc51-46de-83fd-cf49aca62db7)

![image](https://github.com/user-attachments/assets/282bed9d-b2da-4c93-829c-d5338102f77c)

![image](https://github.com/user-attachments/assets/8a4ad68c-83d9-4f36-8601-eea94b6a41e6)


![image](https://github.com/user-attachments/assets/dc8469d4-9cc3-484e-afb8-24797e48f285)

![image](https://github.com/user-attachments/assets/228a0393-7211-4ffb-bc0a-caa2d9318185)


