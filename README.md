# Paypal-payment-using-node.js
In this project ,I will tell you about how to pay the payments using Paypal .I will explain about the set of tools that are used to develop the application
![screenshot 14](https://user-images.githubusercontent.com/26309496/44872599-d53e7e00-ac4a-11e8-9573-6d27e0afb9db.png)**To write an application using SDK we have to follow the certain steps:**

- Register for the developer account and get your client _id and client_secret.
visit the link [https://developer.paypal.com/](url) and login with your Paypal Id.

- Make two accounts one Personnel account that  you will have to use while buying the item through Paypal and the other Business account that will be used as the account that will receive the payment.
Select the country as U.S.A not India otherwise some error can occur as we are using 'sandbox' box for testing purpose not live mode. 
![screenshot 11](https://user-images.githubusercontent.com/26309496/44873610-9100ad00-ac4d-11e8-9c4a-c4cea5502cc6.png)
- Add dependency 'paypal-rest-sdk' in your package.json file.
npm install paypal-rest-sdk  for installing the module using node.js command prompt.
- To get client_id and client_secret <br/>Go to My Apps & Credentials 
![screenshot 13](https://user-images.githubusercontent.com/26309496/44874543-59473480-ac50-11e8-9d8c-8e1cd25bce02.png)

- require paypal-rest-sdk in your file<br/>
-create config options with mode,client_id and client_secret<br/>
paypal.configure({<br/>
  'mode': 'sandbox', //sandbox or live<br/>
  'client_id': 'your client_id',<br/>
  'client_secret': 'your client_secret'<br/>
});

- Framework used:Express.js
Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications. It is an open source framework developed and maintained by the Node.js foundation.

- Middleware used:<br/>

1. body-parser: For parsing the incoming request it is used.It is available under req.body property. 
npm install body-parser.

- View Engine : I have used EJS as a view engine as its syntax is similar to HTML and I find it to be easy as compare to handlebars view engine and jade engine

- Now you can run your server at localhost:3000 and click buy in browser,then you will be redirected to paypal payment gateway and here you have to login with your sandbox personnel account .
![screenshot 15](https://user-images.githubusercontent.com/26309496/44875316-a75d3780-ac52-11e8-8636-23da15be6e2b.png)

- Now you can [visit](https://www.sandbox.paypal.com/) and see if the amount is received in your business account that you have setup in My Apps & Credentials or not.Check if everything is working fine!!
![screenshot 19](https://user-images.githubusercontent.com/26309496/44875413-f30fe100-ac52-11e8-9a85-0f58deee18a3.png)
Thanks
Mohit Sood
I
 
