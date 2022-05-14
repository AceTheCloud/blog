---
layout: post
title: "Java for Azure Developers and Architects (2 of 10)"
img: java.jpg
date: 2021-08-04 12:55:00 +0300
description: Java for Azure Developers and Architects (2 of 10)
tag: [Java, SpringBoot, Azure]
---

# Java for Azure Developers and Architects (Blog 2 of 10)


## The Project Structure

```
   ├───pom.xml            
   ├───src
       ├───main
       │   ├───frontend
       │   ├───java
       │   │   └───com
       │   │       └───baeldung
       │   │           └───ecommerce
       │   │               │   EcommerceApplication.java
       │   │               ├───controller 
       │   │               ├───dto  
       │   │               ├───exception
       │   │               ├───model
       │   │               ├───repository
       │   │               └───service
       │   │                       
       │   └───resources
       │       │   application.properties
       │       ├───static
       │       └───templates
       └───test
           └───java
               └───com
                   └───baeldung
                       └───ecommerce
                               EcommerceApplicationIntegrationTest.java
```



