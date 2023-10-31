# Exercise 1: Create an Application to consume the OnlineShop Purchase Requisition event and update the status of the Purchase Requisition in SAP Build Code

From this exercise on, we will switch to SAP's Business Technology Platform (BTP).

In this exercise, we will consume the event created in the **OnlineShop** app in SAP S/4HANA in the previous chapter. Broadly, there will be two main steps:
- Consume an SAP S/4HANA On-Premise event for **Purchase Requisition Create**, and persist the data in SAP HANA Cloud.
- Add an external API(S/4HANA OP) to read the Purchase Requisition data in SAP BTP.

To create such a scenario, we need to do the following:
1. [Create a project in the SAP Build lobby](exercises/buildcode/exercises/ex1/README.md)
2. [Create a data model for purchase requisition for local persistence and add an external API association ](../../../buildcode/exercises/ex2/README.md)
3. [Create a service ](../../../buildcode/exercises/ex3/README.md)[add and consume an event from S/4HANA On-Premise](../../../buildcode/exercises/ex4/README.md)
4. [Add and consume an event from SAP S/4HANA On-Premise](../../../buildcode/exercises/ex4/README.md)
5. [Create a UI application](../../../buildcode/exercises/ex5/README.md)
6. [Preview and test the app](../../../buildcode/exercises/ex6/README.md)

# Create a new project in the SAP Build lobby.
> Note: Please use Google Chrome or Microsoft Edge to perform the exercises.

1. Open the [SAP Build lobby](https://lcapteched.eu10.build.cloud.sap/lobby) and log in with the provided user ID and password.

2. Click **Create**. A new window opens asking you what you would like to do. 

![](images/Build_001.png)

3. Select **Build an Application**.

![](images/Build_002.png)

4. You are asked which type of application you would like to build. Select **SAP Build Code**.

![](images/CreateProject_BuildCode.png)

5. On the next step, choose **Full Stack Application**. 

![](images/CreateFullStack.png)

6. In the **Create a Full-Stack project** step,
   - In the **Project Name** field, enter *'ManagePurchaseRequisitionXXX'* and replace XXX with the 3-digit number of the user ID that you used for login.
     > Note: Make sure you copy the project name without any spelling mistakes and only replace XXX with the 3-digit username. If the name is changed, you might run into issues in the remaining exercise.
   - In the **Description** field, enter a short description for the project.
   - In the **Namespace** field, enter the namespace of the application's data model.
   - In the **Service Name** field, enter the name of the application's default service.
   - Do not change the recommended dev space name.


> Note: The dev space recommended for you, may be a different from the one in the example. That's OK,  you can proceed.

![](images/ProjectName.png)

It will take some time until your project is created. Once the project is created, you will see it listed in the lobby. 

7. Click on the name of the project to open it in SAP Business Application Studio.
![](images/projectCreated.png)
   

Continue to **[Build Exercise 2: Create Data Model](../../../buildcode/exercises/ex2/README.md)**

