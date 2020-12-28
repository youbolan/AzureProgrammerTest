## Post Sample

Send post request to this url  
    https://azurefuctionprogrammertest.azurewebsites.net/api/PostOrder?code=h/mhs6lAwBqpzIu5jjsmon2q3Gm7knRotEZg297ARjDbKotYOvjwTQ==
    
- PurchseOrderNumber exists in the database, return http status code 204

    ![204 sample](image/204.png)

- BillingZipCode is missing, reject it with http status code 400

    ![400 sample](image/400.png)

- Order is created successfully, return http status code 201

    ![201 sample](image/201.png)
