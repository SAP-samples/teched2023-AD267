
# AD267 - Extending with ABAP Cloud and SAP Cloud Application Programming Model

## Description

This repository contains the material for the SAP TechEd 2023 session called AD267 - Extending with ABAP Cloud and SAP Cloud Application Programming Model.

## Overview

### The Clean Core Strategy
SAP advocates keeping your Core Clean by using the various Extensibility Options given below in the diagram.
We shall make use of Developer Extensibility and Side-by-Side extensibility and show how easy it is to communicate between both worlds in this hands-on exercise.

![](images/CleanCore.png)

### SAP Build Code

Last year, SAP launched SAP Build to empower business experts to construct applications, implement automations and compose business sites. This year, the Build family is being expanded to offer a powerful shortcut for cloud application development with the introduction of SAP Build Code.

![](images/img-build-code-architecture.png)

SAP Build Code unifies essential application development tools such as SAP Business Application Studio, SAP Cloud Application Programming Model (CAP), SAPUI5, SAP Mobile Services, and SAP Document Management Services. It is powered by the generative AI copilot, Joule, and enables interoperability with ABAP Cloud. Additionally, it facilitates seamless collaboration with SAP Build's low-code solutions and provides robust governance and lifecycle management features.

![](images/img-build-code-benefits.png)

### Exercise Overview

In this hands-on session, we will create a new service using the ABAP RESTful Application Programming Model (RAP) in an on-premise SAP S/4HANA system. This RAP service will generate an event which will then be consumed in an application created by you using the Cloud Programming Model (CAP) on the SAP Business Technology Platform (BTP).

## Requirements

To carry out the exercises of this repository, you need to
- use ABAP Development Tools (ADT) for the ABAP development parts
- have a browser ready, preferably Google Chrome, to access SAP Build Code

The users for the development environment during the course are the User IDs that have been provided to you by the hosts.

Go to [Getting Started - Preparation](exercises/ex0/README.md) to find the installation details, and URLs, and then start with the first exercise.

### Business Scenario 

In this hands-on workshop, we will implement an online shop for employees which will allow the creation of *Purchase Requisitions* by using a released RAP facade from Procurements.   
 
 - An existing customer/partner wants to create a new business application that will allow employees of a company to order certain articles such as laptops for quick delivery using this shopping app. Purchase Requisition created can be viewed/approved by an Approver through an application on SAP BTP. This scenario can be realized with ABAP RESTful Application Programming Model (RAP) and SAP Build Code. 
 
 - You’ll build an application starting from a database table using an ADT wizard that generates a starter project which contains all the needed development RAP artefacts that have to be implemented. The generated business service will be transactional, draft-enabled, and enriched with UI semantics for the generation of the Fiori elements app. This application will create a standard Purchase Requisition in S/4HANA On-Premise system.

 - Next, you will move to SAP  Build Code on SAP Business Technology Platform. You will create a Project in SAP Build lobby and use the "Productivity Tools" of SAP Business application Studio. You will use the Storyboard to create a data model, consume external resources (event & external API) from the S/4HANA On-premise, draft enabled service, and finally a UI application. This application will consume "Purchase Requisition Create" event from the S/4HANA OP system and allow you to approve it BTP while storing the data in SAP HANA Cloud.

   
## Exercises

- [Getting Started - Preparation](exercises/ex0/README.md)
- [Part 1 - ABAP ](exercises/rap/README.md)
  - [Exercise 1: Create an ABAP Package](exercises/ex1/README.md)
  - [Exercise 2: Create the OnlineShop Application](exercises/ex2/README.md)
  - [Exercise 3: Adapt the data model](exercises/ex3/README.md)
  - [Exercise 4: Create a Web API for the Onlineshop](../ex4/README.md)
      
- [Part 2 - SAP Build Code](exercises/buildcode/exercises/ex1/README.md)
  - [Build Exercise 2: Create Data Model](exercises/buildcode/exercises/ex2/README.md)
  - [Build Exercise 3: SAP Create Service](exercises/buildcode/exercises/ex3/README.md)
  - [Build Exercise 4: Add and consume an event from S/4HANA On-Premise](exercises/buildcode/exercises/ex4/README.md)
  - [Build Exercise 5: Create UI application](exercises/buildcode/exercises/ex5/README.md)
  - [Build Exercise 6: Preview and test the app](exercises/buildcode/exercises/ex6/README.md)
  
## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support bby creating a new issue via the [Issues](../../issues) tab.

## License
Copyright (c) 2023 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
