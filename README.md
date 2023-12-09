Rainforest Payment Integration Example
Introduction

This repository offers an HTML example for integrating Rainforest Payment into a web page. It utilizes JavaScript to dynamically load the payment script and configure the payment element, allowing for environment-specific settings based on URL parameters.

Features

Dynamic Script Loading: Automatically loads the Rainforest Payment script (production or sandbox) based on the isProd URL parameter.
Configurable Payment Element: The payment element is set up via JavaScript, enabling session key and payin configuration ID specification, and customization of allowed methods and styles.
Setup

Clone the Repository:
Download the repository to your local machine or server:
bash
Copy code
git clone [Your-Repository-URL]
Host the Page:
Deploy the index.html file on a web server, ensuring HTTPS support for security.
Usage

To implement the payment page:

Call to URL: Make a request to your hosted page with the isProd parameter. Example URL format:
ruby
Copy code
https://[your-website]/[path-to-html]?isProd=[true/false]
isProd: Set to true for production environments or false for sandbox testing.
Invoke addPaymentElement: In your JavaScript, call addPaymentElement(sessionKey, payinConfigId) with your specific session key and payin configuration ID values.