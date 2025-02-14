# Web Application Testing

Before starting testing, I prepared a [test plan](https://docs.google.com/spreadsheets/d/1E7wukTPh5yAg577Xa9tHZus5_rivVYvNpHd43OW1NpM/edit?usp=sharing) in which I defined goals, strategies, and testing areas. It describes the methods used, entry and exit criteria, risks.

## Requirements analysis and test documentation preparation:
*[Check list for Cart Management и Order Management modules](https://docs.google.com/file/d/1nYNbIoCG4zT5S-1lTzev2XNLWvrVacWL/edit?usp=docslist_api&filetype=msexcel)
*[Test cases](https://github.com/KseniiaPetrova923/web/blob/main/testcases2.pdf)

## Functional testing:
*[Bug reports](https://github.com/KseniiaPetrova923/web/blob/06c9fc7755522f4ac977b64e52632fa992867656/Issues2.xls)
*[Test run results](https://github.com/KseniiaPetrova923/web/blob/06c9fc7755522f4ac977b64e52632fa992867656/test%20run2.pdf)

## Using of Charles Proxy:
To test the web application, I used a sniffer to intercept, modify and analyze HTTP requests.As part of the training assignment, I completed the following tasks:

1) Changing the number of products in the cart:
Using a breakpoint, I intercepted a request when adding 2 products, changed the data, sending 500 instead of 2 products to the cart.

2) Simulating an access error (403 Forbidden):
I simulated a situation in which the https://demoshopping.ru server returns status code 403, limiting access to the resource, but maintaining the operation of other requests.

3) Redirecting requests from production to the QA stand:
I set up a redirection of requests from https://demoshopping.ru (production) to https://qa.demoshopping.ru (test environment), which made it possible to test functionality without affecting the production version.

[Using of Charles Proxy](https://github.com/KseniiaPetrova923/web/blob/main/Charles%20proxy.zip)
