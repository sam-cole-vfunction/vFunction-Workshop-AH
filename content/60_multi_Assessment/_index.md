---
title: "Multi App Assessment"
chapter: true
weight: 60
---

# Multi App Assessment

ReRun the Assessment for the following applications:

## Petclinic
```
archives:
  - c:\tmp\spring-petclinic-3.0.0-SNAPSHOT.jar
app:
  included_packages:
    - org.springframework.samples.petclinic.
```

## DayTrader
```
archives:
  - c:\tmp\dayrader-ee7.ear
app:
  included_packages:
    - com.ibm.websphere.samples.daytrader.
```


## DhanjyothiBank
```
archives:
  - c:\tmp\DhanjyothiBank-0.0.1-SNAPSHOT.war
app:
  included_packages:
    - com.dhanjyothi.
```

## Minecraft
```
archives:
  - c:\tmp\minecraft.jar
app:
  included_packages:
    - net.minecraft.
```

{{% notice note %}}
Do you think any of the sample apps are suitable for refactoring?
{{% /notice %}}