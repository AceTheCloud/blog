---
layout: post
title: "Java for Azure Developers and Architects ( 1 of 3)"
img: java.jpg
date: 2021-08-03 12:55:00 +0300
description: Java for Azure Developers and Architects (1 of 3)
tag: [Java, SpringBoot, Azure]
---

# Java for Azure Developers and Architects (Blog 1 of 3)

### Why Java on Azure ?

According to Stack Overflow and GitHub, Java is the one of the widely used programming language.
Java Virtual Machine (JVM) offers a easy and secure way to run Java applications efficiently.

Azure offers various ways to deploy your Java applications. No matter what types of Java applications you're running, Azure has a solution. You can choose from batch processes, nanoservices, and microservices, all the way up to Java Enterprise Edition (EE) and Jakarta EE applications

In this series of blog posts, we'll create a very simple e-commerce application. 

### Tech Stack
In terms of basic operations, the user will be able to add/remove products from a product list to/from a shopping cart and to place an order.
Lets name our ecommerce application as "OnlineMart". 
To develop the API, we'll use the latest version of Spring Boot. We also use JPA and Azure MySQL database for the persistence side of things.
We will develop an API using Spring Boot and a client application that will consume the API using Angular.

___

### Java Technologies

#### Spring Framework
The Spring Framework is an application framework and inversion of control (IoC) container. Spring has historically been used to complement the Enterprise JavaBeans (EJB) model. Its core functionalities are:

Dependency injection
Aspect-oriented programming
Business abstraction
Spring Boot
Spring Boot runs on top of the Spring Framework and has an opinionated autoconfiguration. Spring Boot applications run standalone and are a perfect fit for microservices.

#### Spring Data
Spring Data simplifies data access for relational and non-relational databases, map-reduce frameworks, and cloud-based data services.

#### Spring Security
Spring Security is the de facto standard for securing Spring-based applications. It offers a high level of authentication and access control. For instance, Spring Security integrates well with Active Directory.

#### Spring Cloud
Spring Cloud is used for distributed systems. Spring Cloud comes with service discovery, configuration management, monitoring, and a good developer experience.

#### Spring Batch
Spring Batch is a lightweight framework for robust batch applications that are vital for daily operations.

#### MicroProfile and Jakarta EE
MicroProfile and Jakarta Enterprise Edition (EE) can be seen as the open-source follow-up of the Java EE specifications.

MicroProfile is a set of specifications for microservice architectures. It calls itself an open forum to optimize Enterprise Java for a microservices architecture. MicroProfile aims to innovate across multiple implementations and collaborate on common areas of interest.

Jakarta EE is a set of specifications for building enterprise applications. Its modularized structure enables developers to create efficient software solutions. Jakarta EE applications can be packaged as either EAR files or WAR files.

WebProfile is a subset of Jakarta EE for back-end services with a web focus. But don't worry! You can add specific APIs of the enterprise platform on top of it.

#### Application servers
Java EE applications must be deployed onto Java EE-compliant application servers (WebLogic, WebSphere, WildFly, GlassFish, Payara, and others).

Apache Tomcat is an HTTP server and a Java Servlet container. It implements the Servlet, Java Server Pages (JSP), Java Expression Language, and Java WebSocket specifications.

Oracle WebLogic Server is a unified and extensible platform for developing, deploying, and running enterprise applications. WebLogic Server offers a robust, mature implementation of Java EE and Jakarta EE.

Red Hat JBoss Enterprise Application Platform delivers enterprise-grade security and performance for both on-premises and virtual implementations, or in private, public, or hybrid clouds.

WildFly is the open-source upstream for JBoss EAP. This community-driven variety is great for development and testing.

IBM WebSphere Application Server (WAS) is a flexible, security-rich Java server runtime environment for enterprise applications. It focuses on high reliability. It supports microservices and standards-based programming models. You can modernize at your own pace, gain greater visibility across workloads, analyze enterprise applications, and advance your journey to Kubernetes.

Open Liberty is the community-driven, open-source version of WAS.

Oracle GlassFish is the reference implementation of many Java EE web standards (including Servlet and JSP).

___

## Types of Java applications

In this unit, we'll distinguish between the different types of server-side Java applications to help you choose a matching cloud solution.

### Monolithic applications (Azure Infra Solution - Ex : AzureVMs Azure App Service )
A monolithic application is an all in one solution that still fits for many projects. A monolithic application is a good start for prototyping and startups. It's simple to develop, debug, test, and deploy.

Traditionally, monolithic applications run on application servers and scale the entire application as a whole.

### Microservices (Azure Infra Solution - Ex Azure App Service, Azure Container Instances , Azure K8s Service)
Today, in order to succeed, businesses are asked to adapt, fail fast, and expect the unexpected. To achieve a reduced time to market, more engineers get hired. But the outcome might be the opposite! It results in a higher time to market, because you have more communication effort when more engineers need to collaborate. The solution here is to divide and conquer.

In a cross-functional team, you can deliver features as independently as possible. Each team should be responsible for its own dedicated part of the software.

### Batch jobs (Azure Infra Solution - Ex Azure Function, Azure Data Factory, Apache Flink running on Azure VMs)
Some applications are intended to run briefly. They execute a particular workload, and then exit rather than wait for requests or user input. Batch jobs are a solution for this use case. Even though some batches can last for hours, sometimes jobs need to run once or at regular, scheduled intervals.

### Serverless architectures (Azure Infra Solution -  Azure Functions , Azure Logic Apps)
Functions are executed only on an event. A function is "triggered" by a specific type of event. Supported triggers include responding to changes in data, responding to messages, running on a schedule, or receiving an HTTP request.

___

### Azure Spring Cloud
Azure Spring Cloud lets you focus on building Spring Boot apps without managing infrastructure. 
You can easily deploy your JARs or code, and it will automatically wire your apps with the Spring service runtime. 
After you deploy the apps, you can easily monitor their performance, fix errors, and make improvements.
Azure Spring Cloud is integrated into the Azure ecosystem and is ready to tackle enterprise workloads.

Links to other posts of  __Java for Azure Developers and Architects Series__ :
