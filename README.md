# ChainOfResponsibility
Implementation of Chain Of Responsibility Design Pattern

Imagine you are operating an e-commerce system where orders pass through several stages:

  *Validation: To ensure the order details are complete and accurate.
  *Discount Application: To check and apply any available discounts or promotional offers.
  *Payment: To process payment for the order.
  *Shipping: To finally ship the order to the customer.

In this project , once an order is created, it goes through a series of handlers – it is first validated, then any discounts are applied, then processing the payment, and finally, the order is shipped. Each handler decides whether to pass the order to the next handler or halt the process. 
