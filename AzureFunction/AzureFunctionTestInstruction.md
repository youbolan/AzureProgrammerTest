# Azure Functions App Test Instruction

This test usually takes two to three hours to finish all levels if you have the experience. 

You have up to eight hours to finish all levels (Leve 1, Level 2, Leve l3 and Level 4). If don't need to finish all levels, please observe the following deadline:

Level 1: Up to 4.5 hours

Level 2: Up to 5 hours

Level 3: Up to 6.5 hours

Level 4: Up to 8 hours

Time is calculated from the moment we send this test description link to you.

Email your code to qingfeng.tan@hurraymart.com before the deadline. Make sure the code file includes the script to creat the database. If you use Visual Studio to develop the project, zip the whole solution and email the zip file.

If you need to finsh Level 2 ["Publish this Funciton App to Azure"](#level-2--publish-this-funciton-app-to-azure), send the API link with your code together. 

## Level 1: Use C# to create an Azure Functions App with the following two Web APIs.

```diff
- If you don't know how to use Azure Funciton App, you can use ASP.NET Web API.
```

### 1. PostOrder

This API acceptes a http post request and creates the order in SQL database

- Order Structure  

    An order has four fields, BuyerName, PurchseOrderNumber, BillingZipCode, OrderAmount.  

    Here is a json sample: 
    
    ``` json 
    {
	    "BuyerName": "Test User 04",
	
	    "PurchaseOrderNumber" : "Test PO 04",

	    "BillingZipCode" : "40001",

	    "OrderAmount" : 49.99
    }
    ```

- If PurchaseOrderNumber exists in the database, return http status code 204.

- If any field is missing, reject it with a http status code 400.

- If the order is created successfully, return http status code 201.

- PostOrder Sample: [https://github.com/vibesbase-cloud-developer/AzureProgrammerTest/blob/master/AzureFunction/PostSample.md](PostSample.md)

### 2. GetOrders
This API acceptes a http get request and return the list of matched orders. Filters on BuyerName, PurchaseOrderNum and BillingZipCode should also be implemented.

- GetOrders sample: [https://github.com/vibesbase-cloud-developer/AzureProgrammerTest/blob/master/AzureFunction/GetOrdersSample.md](GetOrdersSample.md)
   
  
## Level 2:  Publish this Funciton App to Azure

Publish this Azure Fuctions App, send the Web API link to qingfeng.tan@hurraymart.com with your code together.

## Level 3: Unit Test

### You have two options to write unit test. You only need to choose one to implement.
1. Unit test for the Web API. This may take much more time if you never practiced it before.
2. Unit test for database operation. If you choose this one, make sure you separete the data access code, so you can write unit test.

### Unit test must cover the following cases
1. Successfully insert a new record
2. Cannot insert record with duplicate PurchaseOrderNumber
3. Cannot insert record without BillingZipCode
4. Successfully retrieve an exsiting record


## Level 4 Auto Deploy
Use git as your source code control, for example github, bitbucket, Azure DevOps and gitee etc.
Setup a auto deploy script
Once you push the code, publish the app to Azure automatially. 
