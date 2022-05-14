---
layout: post
title: "Java for Azure Developers and Architects (2 of 15) - Setup Your Environment"
img: java.jpg
date: 2021-08-04 12:55:00 +0300
description: Java for Azure Developers and Architects (2 of 15) - Setup your environment
tag: [Java, SpringBoot, Azure, SpringCloud]
---

# Java for Azure Developers and Architects (Blog 2 of 15)


## Setting up the Environment

In this post, we'll set up everything you need to setup your dev machine.

### Prerequisites
1) JDK 17
2) VSCode with Java Extensions Pack 
3) Git with Azure CLI

Let's run the following command to check the Azure CLI version

```
az --version
```

![Azure CLI output version](/assets/img/2021-08-04-Java-SpringBoot-On-Azure-Cloud-2/AzCLIversion.png "Azure CLI Output")

You can install this extension after installing Azure CLI by running.

```
az extension add -n spring-cloud -y
```

If the extension is already installed, update it to the latest version by running 

```
az extension update -n spring-cloud
```