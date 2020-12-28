## GetOrdersSample

Send GET request to this url  
https://azurefuctionprogrammertest.azurewebsites.net/api/GetOrders?code=O/rucuU0heFhAbUcsk7b9atIVjHcNTumj/qOvLVSb45iYKOcqI0UaQ==

- Without any filter, returns all orders in the database. 
 https://azurefuctionprogrammertest.azurewebsites.net/api/GetOrders?code=O/rucuU0heFhAbUcsk7b9atIVjHcNTumj/qOvLVSb45iYKOcqI0UaQ== 
    ![No Filter](image/NoFilter.png)
- Apply filter on BuyerName, only returns the matched record.
https://azurefuctionprogrammertest.azurewebsites.net/api/GetOrders?BuyerName=Test%20User%2004&code=code=O/rucuU0heFhAbUcsk7b9atIVjHcNTumj/qOvLVSb45iYKOcqI0UaQ==
    ![Filter BuyerName](image/FilterBuyerName.png)
- Apply filter on PurchaseOrderNum, only returns the matched record.
https://azurefuctionprogrammertest.azurewebsites.net/api/GetOrders?PurchaseOrderNumber=Test%20PO%2002&code=O/rucuU0heFhAbUcsk7b9atIVjHcNTumj/qOvLVSb45iYKOcqI0UaQ==
    ![Filter PurchaseOrderNumber](image/FilterPO.png)
- Apply filter on BillingZipCode, only returns the matched record.
https://azurefuctionprogrammertest.azurewebsites.net/api/GetOrders?billingZipCode=30001&code=O/rucuU0heFhAbUcsk7b9atIVjHcNTumj/qOvLVSb45iYKOcqI0UaQ==
    ![Filter BillingZipCode](image/FilterBillingZipCode.png)
