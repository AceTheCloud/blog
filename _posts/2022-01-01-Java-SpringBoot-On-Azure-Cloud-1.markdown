---
layout: post
title: "Java for Azure Developers and Architects ( 1 of 10)"
img: java.jpg
date: 2020-08-03 12:55:00 +0300
description: Java and SpringBoot on Azure Cloud (1 of 10)
tag: [Java, SpringBoot, Azure]
---

# Java for Azure Developers and Architects (Blog 1 of 10)

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
