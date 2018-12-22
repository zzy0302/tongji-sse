# 来自zzy的学院服务器访问指南 v0.0.1 update:2018/12/18
[TOC]

---

## For Windows
### Step1:打开运行 开始菜单右键->运行

### Step2:输入以下内容并回车
	\\10.60.41.1

### Step3:账户名为 'b'+学号+'\_' +姓名拼音 密码为'1234'
例如你是张三，你的学号是114514，那你的账户就是"b114514_zhangsan"
密码均为 "1234"
如何修改密码请参考服务器的指示

---

## For Mac OS
### Step1:打开访达(finder)，按下组合键 
	command+k
### Step2:输入以下内容并回车
	10.60.41.1
### Step3:账户名为 'b'+学号+'\_' +姓名拼音 密码为'1234'
例如你是张三，你的学号是114514，那你的账户就是"b114514_zhangsan"
密码均为 "1234"
如何修改密码请参考服务器的指示
### Step4:任选一个文件夹 我推荐最下面的Publicfiles 这个都有权限，然后点 "好"
### Step5:关闭这个窗口，从访达(finder)左侧找到服务器(10.60.41.1)然后找你需要的目录

## ERROR解决方法
### 没有smb1服务
https://support.microsoft.com/en-sg/help/2696547/how-to-detect-enable-and-disable-smbv1-smbv2-and-smbv3-in-windows-and
看不懂上面的在powershell（管理员）中输入如下的内容

	Enable-WindowsOptionalFeature -Online -FeatureName smb1protocol
	Set-SmbServerConfiguration -EnableSMB1Protocol $true