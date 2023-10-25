
# AD267 - Extending with ABAP Cloud and SAP Cloud Application Programming Model

## Description

This repository contains the material for the SAP TechEd 2023 session called AD267 - Extending with ABAP Cloud and SAP Cloud Application Programming Model.

## Overview

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

## Exercises

- [Getting Started - Preparation](exercises/ex0/README.md)
- [Part 1 - ABAP ](exercises/rap/README.md)
- [Part 2 - SAP Build Code](exercises/buildcode/exercises/ex1/README.md)
  
## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support bby creating a new issue via the [Issues](../../issues) tab.

## License
Copyright (c) 2023 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
