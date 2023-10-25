# Exercise 4: Add and consume an event from S/4HANA On-Premise system
Now you will go to the **Service Center** and add an event to the project.

1. Go to the **Service Center** on the left panel.
![](images/Event_000.png)
![](images/Event_001.png)

3. Open node **SAP Business Accelerator Hub -> SAP S/4HANA -> S4HANABusinessEvents** and search for "Purchase Requisition"
![](images/Event_002.png)

4. Click on Add event button
![](images/Event_009.png)

5. Event is added to the project and is available under "External Resources".
![](images/Event_003.png)

6. Next we will consume this event.
![](images/Event_004.png)

7. This will open the 'Application Logic Editor'.
![](images/Event_010.png)

8. Add logic to insert data in PurchaseRequisition entity.
![](images/Event_005.png)
![](images/Event_006.png)
![](images/Event_007.png)

10. Open Code Editor to view the code
![](images/Event_008.png)
replace the **await** statement code with:
```js
await INSERT .into `ManagePurchaseRequisitionService.PurchaseRequisition` .entries({purchaserequisition:message.data.PurchaseRequisition});
```
Continue to - **[Build Exercise 5: Create UI application](../../../buildcode/exercises/ex5/README.md)**
