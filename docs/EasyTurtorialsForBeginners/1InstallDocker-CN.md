欢迎!本章我们会安装Docker，作为部署的基础。

本教程将教您如何安装Docker。

## 什么是Docker？  
Docker是一款开源的容器技术，它可以让开发者打包他们的应用以及依赖包到一个轻量级、可移植的容器中，然后发布到任何流行的Linux或Windows服务器上，也可以实现虚拟化。容器是完全使用沙箱机制，相互之间不会影响，因此非常适合于开发、测试和部署环境的隔离。

在部署Astra Voice Agent时，我们将使用Docker容器，所以在安装Docker之前，请确保您已经安装了Docker Desktop。

## 安装准备
### 1.确定您的windows版本。
<details>
<summary>如何确定windows版本？</summary>
Windows 徽标键 + R，并在“打开”框中键入“winver”，然后选择“确定”。
如果您是windows专业版用户，则会显示“Windows 专业版”；如果您是windows家庭版用户，则会显示“Windows 家庭版”。
</details>

### 2.安装必要组件
<details>
<summary>如果您是window家庭版系统用户，请参考以下教程。</summary>

##### a.开启虚拟化
首先，您需要开启虚拟化功能。

检查是否已经开启虚拟化：
右键桌面底部的任务栏，单击任务管理器，在如下位置查看虚拟化是否开启：
![1-1.png](pictures%2F1-1.png)

如未开启，参考教程开启：https://www.omicsclass.com/article/367。

##### b.开启Hyper-V
注意！开启hyper-v可能会和虚拟机相关软件冲突！请提前确认！

由于win10家庭版没有Hyper-V选项，需要用如下方法设置：

打开此链接
</details>

<details>
<summary>如果您是window专业版系统用户，请参考以下教程。</summary>

</details>





如果您是windows家庭版用户（如何区分）
## 下载Docker Desktop
打开网站 https://www.docker.com/get-started ，选择适合您的操作系统的安装包，下载并安装Docker Desktop。

## 安装Docker  
Docker可以安装在Linux、Windows和Mac上。

### Windows 安装教程

# 参考资料
- [什么是Docker？](https://www.docker.com/resources/what-is-docker)
- [Win10家庭版也可以装Docker桌面版了！](https://www.omicsclass.com/article/1243)