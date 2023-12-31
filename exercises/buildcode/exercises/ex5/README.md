# Exercise 5: Create UI Application
After defining the foundation of your application in the previous chapter, we will add an SAP Fiori elements based User Interface to the application.

1. Go to the storyboard page and find the UI Applications tile and choose the + icon to add a new user interface.
![](images/UI_001.png)

2. A screen will show up where you can add the Display Name: ManagePurchaseRequisition-<Your-User-ID> and enter a description. Choose Next.
![](images/UI_002.png)

3. Select UI Application type as Template-Based, Responsive Application to create a SAP Fiori elements based UI. Choose Next.
![](images/UI_003.png)

4. Choose UI application template as List Report Page. Choose Next.
![](images/UI_004.png)

5. Select PurchaseRequisition as the main entity in Data Objects, to show PurchaseRequisition entity on UI. Choose Finish.
![](images/UI_005.png)

6. Page Map will open automatically in a few seconds. If not, go to Storyboard to find the tile UI Applications and click on *Manage Purchase Requisition* to select "Open in Page Map".
![](images/UI_006.png)
   
7. In the Page Map, find the List Page entry and choose the edit icon.
![](images/UI_007.png)
   
8. Add the following fields to the list page by clicking on the + near Columns
   ![](images/Plus.png)

9. Click on Add Basic Columns
![](images/AddBasic.png)

10. Add the following columns:
- Purchase Requisition
- PurReqnDescription
- _PurchaseRequisitionItem/PurchasingDocument

![](images/ListPageCols.png)

> Note: Though Purchasing Document is an item-level field, it is used on list page to keep it simple for the use case. It has 1:n relationship with Purchase Requisition number.

11. Find the Object Page entry and choose the edit icon.

![](images/UI_009.png)

12. Expand the **Header** section and add a Form Section and name it "Purchase Requisition".

![](images/HeaderForm_001.png)
![](images/HeaderForm_002.png)

13. Next add Basic Fields.
![](images/HeaderForm_003.png)

14.  Add the field 'Purchase Requisition' in *Header Sections*
![](images/HeaderForm_004.png)
![](images/UI_010.png)

15. In **Sections** -> *General Information* -> Form -> Fields, add the following fields
- PurReqnDescription
- PurchaseRequisitionType

![](images/ObjectCols.png)

16. Next, choose the + icon next to Sections to add a new section. In the dropdown, select Add Form Section.

![](images/UI_012.png)

![](images/AddForm.png)
    
 
17. In the popup enter Label as "Item Details".
![](images/UI_013.png)
 
18. Click on Add button to save.

19. In the Sections, open "Items Details". Choose the + icon on the right side of "Form" -> "Fields", to add new fields to Item Details. In the popover, select "Add Basic Columns".
![](images/UI_015.png)  

20. Select the following fields:
- purchaseReqn/_PurchaseRequisitionItem/Material
- purchaseReqn/_PurchaseRequisitionItem/PurchaseRequisitionItemText
- purchaseReqn/_PurchaseRequisitionItem/RequestedQuantity
- purchaseReqn/_PurchaseRequisitionItem/BaseUnit
- purchaseReqn/_PurchaseRequisitionItem/Plant
- purchaseReqn/_PurchaseRequisitionItem/Supplier
![](images/UI_014.png)    
![](images/UI_017.png)  


Continue to - **[Build Exercise 6: Preview and test the app](../../../buildcode/exercises/ex6/README.md)**
