
# Intercept HTTP traffic with Burp Proxy

A brief description of what this project does and who it's for

Intercepting a request
Burp Proxy lets you intercept HTTP requests and responses sent between Burp's browser and the target server. This enables you to study how the website behaves when you perform different actions.

Step 1: Launch Burp's browser
Go to the Proxy > Intercept tab.

Click the Intercept is off button, so it toggles to Intercept is on.

Intercept is on
Click Open Browser. This launches Burp's browser, which is preconfigured to work with Burp right out of the box.

Position the windows so that you can see both Burp and Burp's browser.


Step 2: Intercept a request
Using Burp's browser, try to visit https://portswigger.net and observe that the site doesn't load. Burp Proxy has intercepted the HTTP request that was issued by the browser before it could reach the server. You can see this intercepted request on the Proxy > Intercept tab.

Viewing an intercepted request in Burp Proxy
The request is held here so that you can study it, and even modify it, before forwarding it to the target server.

Step 3: Forward the request
Click the Forward button several times to send the intercepted request, and any subsequent ones, until the page loads in Burp's browser.

Step 4: Switch off interception
Due to the number of requests browsers typically send, you often won't want to intercept every single one of them. Click the Intercept is on button so that it now says Intercept is off.

Proxy Intercept is off
Go back to the browser and confirm that you can now interact with the site as normal.

Step 5: View the HTTP history
In Burp, go to the Proxy > HTTP history tab. Here, you can see the history of all HTTP traffic that has passed through Burp Proxy, even while interception was switched off.

Click on any entry in the history to view the raw HTTP request, along with the corresponding response from the server.

![Alt text](https://res.cloudinary.com/dceb4nzy9/image/upload/v1716140962/hxo2k3dsa3a8pu6nuvjp.png)

Viewing the HTTP history in Burp Proxy
This lets you explore the website as normal and study the interactions between Burp's browser and the server afterward, which is more convenient in many cases.