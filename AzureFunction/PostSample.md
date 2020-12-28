## PostOrder Sample

Send post request to this url  
    https://azurefuctionprogrammertest.azurewebsites.net/api/PostOrder?code=wg1yd6lkFOsund3n4KxoqPqA3KoRTj61pEj8ve4nWeaC4XD8lakjOA==
    
- PurchseOrderNumber exists in the database, return http status code 204

    ![204 sample](image/204.png)

- BillingZipCode is missing, reject it with http status code 400

    ![400 sample](image/400.png)

- Order is created successfully, return http status code 201

    ![201 sample](image/201.png)
