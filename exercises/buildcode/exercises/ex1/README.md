# Exercise 1: Create Application to consume OnlineShop Purchase Requisition event and trigger Purchase Order creation

From this exercise on, we will switch to SAP's Business Technology Platform (BTP).

In this exercise we will consume the event created in OnlineShop app in S/4HANA from the previous chapter. Broadly there will be three main steps:
- Consume an S/4HANA On-Premise event for Purchase Requisition Create and persist the data in HANA cloud
- Add an external API(S/4HANA OP) to read Purchase Requisition data in BTP

To create such a scenario we need to do the following:
1. [create a project in SAP Build Lobby](exercises/buildcode/exercises/ex1/README.md)
2. [create data model for purchase requisition for local persistence and add an external API association ](../../../buildcode/exercises/ex2/README.md)
3. [Create Service](../../../buildcode/exercises/ex3/README.md)[add and consume an event from S/4HANA On-Premise](../../../buildcode/exercises/ex4/README.md)
4. [add and consume an event from S/4HANA On-Premise](../../../buildcode/exercises/ex4/README.md)create service
5. [create UI application](../../../buildcode/exercises/ex5/README.md)
6. [preview and test the app](../../../buildcode/exercises/ex6/README.md)

# Create a new Project in the SAP Build Lobby
Hint: Please use Google Chrome or Microsoft Edge to follow the exercises
[SAP Build Apps Lobby](https://lcapteched.eu10.build.cloud.sap/lobby)
1. Open the SAP Build Lobby and login with the provided user-id and password.

2. In the SAP Build Lobby choose the button Create to start
![](images/Build_001.png)

3. A new window opens asking you what you would like to do. Select Build an Application.
![](images/Build_002.png)

4. You are asked which type of application you would like to build. Select SAP Build Code.
![](images/CreateProject_BuildCode.png)

5. On the next step, choose Full Stack Application 
![](images/CreateFullStack.png)

6. Add a Project Name, Namespace, Service Name and a Short Description. Please name the project *'ManagePurchaseRequisitionXXX'* and replace XXX with the 3-digit number as given in your user-id that you used for login. Do not change the recommended dev space name.
![](images/ProjectName.png)

7. It will take some time until your project is created. Once the project is created, you will see it listed in the Lobby. Click on the name of the project to open SAP Business Application Studio.
![](images/projectCreated.png)
   

Continue to - **[Build Exercise 2: Create Data Model](../../../buildcode/exercises/ex2/README.md)**

