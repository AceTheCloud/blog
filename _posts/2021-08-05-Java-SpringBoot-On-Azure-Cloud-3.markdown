---
layout: post
title: "Java for Azure Developers and Architects (3 of 15) - Creating Azure Spring Cloud Instance"
img: java.jpg
date: 2021-08-05 12:55:00 +0300
description: Java for Azure Developers and Architects (3 of 15) - Creating Azure Spring Cloud Instance
tag: [Java, SpringBoot, Azure, SpringCloud]
---

# Java for Azure Developers and Architects (Blog 3 of 15) - Creating Azure Spring Cloud Instance

In this post, we'll create an Azure Spring Cloud instance using Azure CLI. 
You can also do this through Azure Portal, While there are other ways of creating Azure resources, Azure CLI is the quickest and simplest method.

### Verify Azure Subscription

```
az login # Sign into an azure account
az account show # See the currently signed-in account.
```
If you have more than one subscription like me , run following command to set specific subscription as the main subscription and

```
az account set --subscription <SUBSCRIPTION_ID>
```

![set default azure subscription](2021-08-05-Java-SpringBoot-On-Azure-Cloud-3/setAzureAccount.png "set default azure subscription")


### Create an Azure Spring Cloud instance

lets initialize following two variables (choose your own names here)

```
$AZ_RESOURCE_GROUP = "acethecloud-spring-cloud-rg"
$AZ_SPRING_CLOUD_NAME = "acethecloud-spring-cloud"
```

With these variables set, we can now create the Azure Resource group and  Azure Spring Cloud instance.

```
az group create --name $AZ_RESOURCE_GROUP --location westus
```
```
az spring-cloud create -g "$AZ_RESOURCE_GROUP" -n "$AZ_SPRING_CLOUD_NAME" --sku standard
```

above command may take few seconds/minutes and then you can see output similar to the following output:
![create spring cloud instance on azure](2021-08-05-Java-SpringBoot-On-Azure-Cloud-3/SpringCloudCreation.png "create spring cloud instance on azure")

This is how it will be visible inside the Azure Portal instance
![Spring Cloud in Portal](2021-08-05-Java-SpringBoot-On-Azure-Cloud-3/SpringCloudinPortal.png "Spring Cloud in Portal")

Run the following commands, so that we will be running Azure CLI commands referencing the same resource group and Azure Spring Cloud instance. So let's set them as defaults, so we don't have to specify them again

```
az configure --defaults group=$AZ_RESOURCE_GROUP
az configure --defaults spring-cloud=$AZ_SPRING_CLOUD_NAME
```






