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

5. Select main entity PurchaseRequisition as main entity in Data Objects, to show PurchaseRequisition entity on UI. Choose Finish.
![](images/UI_005.png)

6. Page Map will open automatically in few seconds. If not, goto Storyboard to find the tile UI Applications and click on *Manage Purchase Requisition* to select "Open in Page Map".
![](images/UI_006.png)
   
7. Find the List Page entry and choose the edit icon.
![](images/UI_007.png)
   
8. Add the following fields to thh list page

- Purchase Requisition
- purchaseReqn/PurReqnDescription
- Status
- Comments
- purchaseReqn/_PurchaseRequisitionItem/PurchasingDocument
![](images/UI_008.png)
> Note: Though Purchasing Document is an item level field, it is used on list page to keep it simple for the use case. It has 1:n relationship with Purchase Requisition number.

9. Find the Object Page entry and choose the edit icon.
![](images/UI_009.png)

10. Expand the **Header** section and add field 'Purchase Requisition' in *Header Sections*
![](images/UI_010.png)

11. In **Sections** under *General Information* add the following fields
- purchaseReqn/PurReqnDescription
- Comments
![](images/UI_011.png)

12. Next, choose the + icon to add new section to the UI. In the dropdown, select Add Form Section.
![](images/UI_012.png)
 
13. In the popup enter Label as Item Details.
![](images/UI_013.png)
 
14. Click on Add button to save.

15. In the Sections, open "Items Details". Choose the + icon on right side of "Fields", to add new fields to Item Details. In the popover, select "Add Basic Columns".
![](images/UI_015.png)  

16. In the dropdown choose the following fields inside *purchaseReqn/_PurchaseRequisitionItem*

- Material
- ItemText
- Ordered Quantity
- Base UoM
- Supplier
![](images/UI_014.png)    
![](images/UI_016.png)  


Continue to - **[Build Exercise 6: Test](../../../buildcode/exercises/ex6/README.md)**
