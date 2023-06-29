---
title: "Run the Assessment" #
chapter: false
weight: 25
---

## Run the Assessment

We will use the vFunction workshop sandbox to complete the assessment, connect to the Windows VM.

1)	Use Notepad to edit the myapp.yaml file (C:\tmp\myapp.yaml). Add the names of each binary to assess one per line and the packages/classes to include in the assessment.

```
---
archives:
  - c:\tmp\fineract-provider-1.5.1-55949bf8.jar
app:
  included_packages:
    - org.apache.fineract.
```

![image](/images/AH-OffA-Edit.png)

2)	Save the file
3)	Use the viper-cli.bat script to perform the assessment. Open a new command window, navigate to c:\temp and run viper-cli.bat. This will use the myapp.yaml file as input and create a .json file with the output.

![image](/images/AH-OffA-Run.png)

The assessment is completed, we can now upload the results in the vFunction UI to see the results.
