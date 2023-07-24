---
title: "Create a workspace"
chapter: false
weight: 20
---


First we create a new application in vFunction for the application we will assess for Modernization.


1)	In the vFunction UI, Click the ‘My Dashboard’ Menu top left and select ‘Add Application’ (You might need to close any open pop-ups first using the X)

![New App](/images/AH_New_Menu1.png)

2)	In the dialog box add the application name, select the type and add the classes to include in the assessment. You can add multiple package names if needed. Only the applications core packages should be included.
```
Name=OMS.NET
Type=.net
Packages=OMS.
```
![New App](/images/AH_NET_Create.png)

3)	Click ‘Create’ to add the new application

4)	vFunction will create the new application and present a dialog with instructions for adding an agent to the application. This agent can be used to perform both Static and Dynamic analysis. As we are going to run an online assessment we will use this in the next step. 

![New App](/images/AH_NET_Controller.png)

