# Integrate-Payments-Payment-API-Node.js

The Integrate Payments payment API (formerly direct post) node.js example can be used with our payments API directly or through our Collect.js javascript payment integration framework product.

If a developer uses Collect.js then the following parameters (ccnumber, ccexp, cvv) will need to be replaced with "payment_token"
If using Collect.js a Public tokenization key will need to be created in our UAT environment first and published on a website or web application to generate a "payment_token" from the end user cardholder data which will need to be inputted and captured using Collect.js and then passed through our Payment API.

A developer will need to create a private "security_key" to use the Payment API which can be created in our public Sandbox by going into the settings and then clicking the security key link.

PUBLIC SANDBOX : https://www.integratepayments.com/payment-integration-platform

You can view all our documentation at : developer.integratepayments.com 

Teleport directly to our Payment API documenatation : 

https://integratepayments.transactiongateway.com/merchants/resources/integration/integration_portal.php?tid=d86b9b1ef11dfee0abfdf48e0258ab13#methodology

Teleport directly to our Collect.js documenatation : (Only Required if Using Collect.js)

https://integratepayments.transactiongateway.com/merchants/resources/integration/integration_portal.php?tid=d86b9b1ef11dfee0abfdf48e0258ab13#cjs_methodology

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

If you have any questions or need any assistance please email any inquires to : info@integratepayments.com 
