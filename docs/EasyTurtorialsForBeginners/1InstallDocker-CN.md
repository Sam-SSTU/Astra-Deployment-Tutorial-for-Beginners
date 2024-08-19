# 欢迎!本章我们会安装Docker，作为部署的基础。

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
<summary><strong><span style="font-size: 1.2em;">如果您是window家庭版系统用户，请先参考以下教程。</span></strong></summary>

**a.升级到Windows 10/11专业版：**

请注意！任何升级操作都存在风险！请务必谨慎操作！

**b.如果不想升级，可以尝试这篇文章：**[Win10家庭版也可以装Docker桌面版了！](https://www.omicsclass.com/article/1243)

若您安装该教程安装，请直接跳转到 [此处](#justify)

</details>

<details>
<summary><strong><span style="font-size: 1.2em;">如果您是已经是window专业版系统用户，或者已经完成上述教程，请继续请参考以下教程。</span></strong></summary>

##### a.开启虚拟化
首先，您需要开启虚拟化功能。

检查是否已经开启虚拟化：
右键桌面底部的任务栏，单击任务管理器，在如下位置查看虚拟化是否开启：
![1-1.png](pictures%2F1-1.png)

如未开启，参考教程开启：[教程](https://www.omicsclass.com/article/367)

##### b.开启Hyper-V
注意！开启hyper-v可能会和虚拟机相关软件冲突！请提前确认！

`补充一点，如果windows安装docker后发现vm虚拟机挂了，请参考此 [链接](https://blog.51cto.com/u_13673282/5237941)
或者将vmware升级为最新版本`

搜素“控制面版” --> 程序和功能 --> 启用或关闭windows功能 --> 勾选Hyper-V --> 确定 --> 重启电脑。
![1-3.png](pictures%2F1-3.png)
![1-4.png](pictures%2F1-4.png)
切记Hyper-V设置里的所有选项都要打上对勾打开。设置完成后要重启电脑。

##### c.下载Docker Desktop
重启电脑后，打开网站 https://www.docker.com/get-started ，选择适合您的操作系统的安装包，下载并安装Docker Desktop。


##### d.安装完成后，启动Docker Desktop
![1-5.png](pictures%2F1-5.png)

点击启动按钮，等待Docker Desktop启动完成。
</details>

<span id='justify'>
</span>

### 3.验证安装
Windows 徽标键 + R，并在“打开”框中键入“cmd”，然后选择“确定”。

打开命令提示符（cmd），输入docker命令，如果出现docker的输出，则说明安装成功。
示例：
![1-2.png](pictures%2F1-2.png)


# 参考资料
- [什么是Docker？](https://www.docker.com/resources/what-is-docker)
- [Win10家庭版也可以装Docker桌面版了！](https://www.omicsclass.com/article/1243)
