# ChainOfResponsibility
Implementation of Chain Of Responsibility Design Pattern

This is an e-commerce system where orders pass through several stages:

  * Validation: To ensure the order details are complete and accurate.
  * Discount Application: To check and apply any available discounts or promotional offers.
  * Payment: To process payment for the order.
  * Shipping: To finally ship the order to the customer.

In this project , once an order is created, it goes through a series of handlers – it is first validated, then any discounts are applied, then processing the payment, and finally, the order is shipped. Each handler decides whether to pass the order to the next handler or halt the process. 

# When to Use Chain of Responsibility Design Pattern in Real-Time Applications?

* Decoupling is Needed: When the sender of a request should be decoupled from its receiver, Chain of Responsibility offers a way to do this. The sender doesn’t need to know anything about who handles the request.
* Multiple Objects May Handle the Request: Instead of prescribing a specific handler, the request gets passed along a chain until an object handles it or reaches the end of the chain.
* Dynamic Handling: If your application requires flexibility in determining which objects handle requests and how they do so, the Chain of Responsibility allows you to assign and change handlers dynamically.
* Hierarchical Decision Making: In scenarios where decision-making is organized hierarchically (for example, managerial approval processes), this pattern can move a request up the chain until an entity with the appropriate authority handles it.
* Handling Should be Configurable: If you want your system’s users (or administrators) to dynamically configure how requests are handled or in which order, a Chain of Responsibility can be suitable.
* Reduce Direct Links Between Objects: If you want to reduce the direct connections between objects to make the system more modular and easier to maintain, this pattern can help.
Middleware and Filters: This pattern is commonly used in middleware (like in HTTP request processing), where various tasks like authentication, logging, and data processing are done in a chain.
