
# Welcome! In this chapter, we will install Docker as the foundation for deployment.

This tutorial will teach you how to install Docker.

## What is Docker?  
Docker is an open-source container technology that allows developers to package their applications and dependencies into a lightweight, portable container. This container can then be deployed on any popular Linux or Windows server, and it can also achieve virtualization. Containers are completely sandboxed from each other, making them ideal for isolating development, testing, and deployment environments.

When deploying the Astra Voice Agent, we will use Docker containers, so before installing Docker, please ensure that you have installed Docker Desktop.

## Installation Preparation
### 1. Determine your Windows version.
<details>
<summary>How to determine the Windows version?</summary>
Press the Windows logo key + R, type "winver" in the "Open" box, and then select "OK".
If you are using Windows Professional, it will display "Windows Professional"; if you are using Windows Home, it will display "Windows Home".
</details>

### 2. Install the necessary components
<details>
<summary><strong><span style="font-size: 1.2em;">If you are a Windows Home user, please refer to the following tutorial first.</span></strong></summary>

**a. Upgrade to Windows 10/11 Professional:**

Please note! Any upgrade operation carries risks! Please proceed with caution!

**b. If you do not wish to upgrade, you can try this article:** [Windows 10 Home edition can also install Docker Desktop!](https://www.omicsclass.com/article/1243)

If you have installed according to that tutorial, please skip to [this section](#justify).

</details>

<details>
<summary><strong><span style="font-size: 1.2em;">If you are already using Windows Professional, or have completed the above tutorial, please continue with the following instructions.</span></strong></summary>

##### a. Enable Virtualization
First, you need to enable virtualization.

Check if virtualization is enabled:
Right-click the bottom of the desktop taskbar, click Task Manager, and check if virtualization is enabled in the following location:
![1-1.png](pictures%2F1-1.png)

If not enabled, refer to this tutorial to enable it: [Tutorial](https://www.omicsclass.com/article/367).

##### b. Enable Hyper-V
Note! Enabling Hyper-V may conflict with virtual machine-related software! Please confirm in advance!

`Additionally, if you find that VMware is not working after installing Docker on Windows, refer to this [link](https://blog.51cto.com/u_13673282/5237941) or upgrade VMware to the latest version.`

Search "Control Panel" --> Programs and Features --> Turn Windows features on or off --> Check Hyper-V --> OK --> Restart the computer.
![1-3.png](pictures%2F1-3.png)
![1-4.png](pictures%2F1-4.png)
Make sure all options under Hyper-V are checked. After setting, you need to restart the computer.

##### c. Download Docker Desktop
After restarting your computer, open the website https://www.docker.com/get-started, choose the installation package suitable for your operating system, download, and install Docker Desktop.

##### d. After installation, start Docker Desktop
![1-5.png](pictures%2F1-5.png)

Click the start button and wait for Docker Desktop to start.

</details>

<span id='justify'>
</span>

### 3. Verify Installation
Press the Windows logo key + R, type "cmd" in the "Open" box, and then select "OK".

Open the command prompt (cmd), type the docker command, and if you see docker output, the installation was successful.
Example:
![1-2.png](pictures%2F1-2.png)

# References
- [What is Docker?](https://www.docker.com/resources/what-is-docker)
- [Windows 10 Home edition can also install Docker Desktop!](https://www.omicsclass.com/article/1243)
