# Integrate-Payments-Payment-API-Node.js
The Integrate Payments payment API direct post node example can be used with our payments API directly or through our Collect.js product.
If a developer uses Collect.js then the following parameters (ccnumber, ccexp, cvv) will need to be replaced with "payment_token"
A Public tokenization key will need to be created in our UAT environment and published on a website or web application to generate a "payment_token" which will need to be captured first using Collect.js and then passed through the Payments API.

A developer will then need to create a private security key to use the Payments API which can be created in our public Sandbox.

PUBLIC SANDBOX : https://www.integratepayments.com/payment-integration-platform

You can view our documentation at : developer.integratepayments.com 

Payment Token Value	Test Data :

payment_token : 00000000-000000-000000-000000000000	

Credit Card Value Test Data :

ccnumber : 4111111111111111 
ccexp : 1025 
cvv : 999

The parameters will need to be sent through the payment gateway as Query String Parameters in order properly process a transaction for authorization.

type=sale&amount=3.00&ccnumber=4111111111111111&ccexp=1020&cvv=123

OR

type=sale&amount=3.00&payment_token=00000000-000000-000000-000000000000
