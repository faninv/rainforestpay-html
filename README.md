Rainforest Payment Integration Example

Introduction

This repository contains an example HTML file that demonstrates how to integrate the Rainforest Payment system into a web page. It dynamically configures the payment system based on URL parameters, allowing for a flexible and secure payment process.

Features

Dynamically loads Rainforest Payment script (production or sandbox version) based on URL parameters.
Configures payment session key and configuration ID via URL parameters.
Customizes payment button styles and allowed payment methods.
Setup

Clone the Repository: First, clone this repository to your local machine or server where you plan to host the page.
bash
Copy code
git clone [Your-Repository-URL]
Host the Page: Host the index.html file on a server. Ensure that the server supports HTTPS to maintain security standards.
Usage

To use the payment page:

Navigate to the Page: Use a URL that includes the necessary parameters. The format should be:
ruby
Copy code
https://[your-website]/[path-to-html]?sessionKey=[yourSessionKey]&payinConfigId=[yourConfigId]&isProd=[true/false]
sessionKey: Your payment session key.
payinConfigId: Your payment configuration ID.
isProd: Set to true for production environment or false for sandbox testing.
Payment Interface: The payment interface will be configured based on the provided parameters.
Customization

You can customize the appearance and behavior of the payment button by modifying the attributes in the <rainforest-payment> tag. Currently available customizations include:

style-button-color: Hex color code for the button.
style-button-border-radius: Border radius for the button.
style-font-family: Font family for the text inside the button.
For more advanced customizations, you can modify the HTML and JavaScript code according to your needs.

Support

For any issues or questions, please open an issue on this GitHub repository, and we'll be happy to assist.

Additional Notes:
Replace [Your-Repository-URL] with the actual URL of your GitHub repository.
Replace [your-website] and [path-to-html] with the appropriate website address and path where your HTML file is hosted.
Ensure the instructions are clear and easy to follow for users who might be unfamiliar with web development concepts.