---
title: "Run Assessment"
chapter: false
weight: 30
---



1)	In the vFunction UI, Click the ‘My Dashboard’ Menu top left and select ‘OMS.NET’ (You might need to close any open pop-ups first using the X), You will be presented with the Controller install instructions. If they don't come up click the 'Install Controller' option in the left panel.

![New App](/images/AH_Menu_oms.png)

2)	In the dialog box copy the items as 'Use the following information in order to fill in the template'

3)	Open the vFunction controller installation yaml file using notepad 

```
C:\vFunctionLab\vfunction\config\installation\instances\default-dotnet\installation.yaml
```

4)	Paste the configuration from step 2 over the default items

```
controller:
	name: OMSNET
	host: http://172.2.0.4
	org_id: [Your org_id]
	app_id: [Your app_id]
	client_id: [Your client_id]
	client_secret: [Your client_secret]
```

5)	Change the agent version to framework
```
version: framework
```

6)	Add the path to the OMS.NET Binaries 

```
    - C:\tmp\vfunction-oms-net\OMS.NET\bin
```

7)	Your configuration should look something like this:


![New App](/images/AH_installyaml.png)

8)	Open PowerShell as an administrator and move to the folder: C:\vFunctionLab\vfunction\controller-installation

```
cd C:\vFunctionLab\vfunction\controller-installation
```

9)	Run the command to install the controller

```
.\install.ps1 default-dotnet

```

![New App](/images/AH_controllerinstall.png)


10)	Back in the vFunction UI you should see the new controller active:

![New App](/images/AH_controller_up.png)

11) Click View Assessment Report to see the results (This may take a few mins to process, if the icon is not enabled after a few mins use windows services to restart the vFunction Viper Service)


![New App](/images/AH_netassessment.png)
