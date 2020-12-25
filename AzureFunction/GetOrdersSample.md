## GetOrdersSample

Send GET request to this url  
https://azureprogrammertest.azurewebsites.net/api/GetOrders?code=kuIRSoezYc/IpAVszJZz2jDlxiywOjnIg4uHYaA1aM1A6v9xeH0tCQ==

- Without any filter, returns all orders in the database. 
 https://azureprogrammertest.azurewebsites.net/api/GetOrders?code=kuIRSoezYc/IpAVszJZz2jDlxiywOjnIg4uHYaA1aM1A6v9xeH0tCQ== 
    ![No Filter](image/NoFilter.png)
- Apply filter on BuyerName, only returns the matched record.
https://azureprogrammertest.azurewebsites.net/api/GetOrders?BuyerName=Test%20User%2004&code=kuIRSoezYc/IpAVszJZz2jDlxiywOjnIg4uHYaA1aM1A6v9xeH0tCQ==
    ![Filter BuyerName](image/FilterBuyerName.png)
- Apply filter on PurchaseOrderNum, only returns the matched record.
https://azureprogrammertest.azurewebsites.net/api/GetOrders?PurchaseOrderNumber=Test%20PO%2002&code=kuIRSoezYc/IpAVszJZz2jDlxiywOjnIg4uHYaA1aM1A6v9xeH0tCQ==
    ![Filter PurchaseOrderNumber](image/FilterPO.png)
- Apply filter on BillingZipCode, only returns the matched record.
https://azureprogrammertest.azurewebsites.net/api/GetOrders?billingZipCode=30001&code=kuIRSoezYc/IpAVszJZz2jDlxiywOjnIg4uHYaA1aM1A6v9xeH0tCQ==
    ![Filter BillingZipCode](image/FilterBillingZipCode.png)
