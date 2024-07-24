- Customer Placing an Order: User, Order, Product
- Picking Algorithm: Order, Product
- Picking Orders: Order, Product
- Dropping Orders in Warehouse: Order, Warehouse
- Sorting Based on Destination: Order, Warehouse, Destination
- Distribution Between Warehouses: Order, Warehouse
- Splitting Orders Between Delivery Workers: Order, DeliveryWorker
- Delivery Routing Algorithm: Order, DeliveryWorker, Route
- Confirmation of Client: Order, User
- Client Feedback: User, Order, Feedback
- Tracking Orders Subsystem: Order, OrderTracking
  
## Customer Placing an Order

- User: The individual who places the order.
-Order: Represents the request made by the user, including details like order ID, date, and status.
- Product: The items included in the order, with attributes such as product ID, name, quantity, and price.
-Explanation: The user selects products and submits an order through the application. This step captures user details and the products they wish to purchase.

## Picking Algorithm

- Order: Contains information about the items to be picked.
- Product: The specific items in the order that need to be located and picked.
- Explanation: The algorithm determines the most efficient way to pick items for an order, often considering factors like location in the warehouse and picking speed.

## Picking Orders

- Order: The order that is being processed.
- Product: The products that are being picked from inventory to fulfill the order.
- Explanation: This step involves physically collecting the items from the warehouse shelves based on the order requirements.

## Dropping Orders in Warehouse

- Order: The order being handled.
- Warehouse: The location where the picked items are dropped off for further processing.
- Explanation: After picking, the order items are placed in a designated area within the warehouse for sorting or staging before delivery.

## Sorting Based on Destination

- Order: The order that needs to be sorted.
- Warehouse: The facility where sorting occurs.
- Destination: The final delivery location or area where the order will be sent.
- Explanation: Orders are sorted based on their delivery destinations to streamline the delivery process and ensure that items are grouped efficiently.

## Distribution Between Warehouses

- Order: The order being distributed.
- Warehouse: The warehouses involved in the distribution process.
- Explanation: Orders may be distributed among multiple warehouses to optimize logistics and reduce delivery times based on factors like location and order volume.

## Splitting Orders Between Delivery Workers

- Order: The order that is being split for delivery.
- DeliveryWorker: The individuals responsible for delivering the orders.
- Explanation: Orders are divided among delivery workers based on criteria such as distance, order size, and delivery route to ensure efficient delivery.

## Delivery Routing Algorithm

- Order: The order that needs to be delivered.
- DeliveryWorker: The delivery personnel assigned to the order.
- Route: The path or route taken to deliver the order.
- Explanation: The algorithm calculates the optimal delivery route for the delivery worker, considering factors like traffic, distance, and delivery deadlines.

## Confirmation of Client

- Order: The order being confirmed.
- User: The customer who placed the order.
- Explanation: After the order is delivered, confirmation is sought from the client to verify that the order was received correctly and in good condition.

## Client Feedback

- User: The customer providing feedback.
- Order: The order related to the feedback.
- Feedback: The comments or ratings provided by the user regarding their order experience.
- Explanation: Clients provide feedback on their order experience, which can be used for quality improvement and addressing any issues.

## Tracking Orders Subsystem

- Order: The order being tracked.
- OrderTracking: The system or records used to monitor the order’s status and location throughout the delivery process.
- Explanation: This subsystem provides real-time updates on the order’s status, allowing users to track their orders from placement to delivery.
