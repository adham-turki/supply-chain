## Route
### Attributes:

- routeId: Unique identifier for the route.
- deliveryId: The delivery associated with this route.
- startLocation: Starting point of the route.
- endLocation: Ending point of the route.
- path: Array of locations representing the route.
- estimatedTime: Estimated time to complete the route.
- distance: Total distance of the route.
### Relationships:

- Delivery: Each Route is associated with one Delivery.
- Subroute: A Route can have multiple Subroutes.
## Subroute
### Attributes:

- subrouteId: Unique identifier for the subroute.
- routeId: The route to which this subroute belongs.
- startLocation: Starting point of the subroute.
- endLocation: Ending point of the subroute.
- distance: Distance covered by this subroute.
- estimatedTime: Estimated time to cover this subroute.
### Relationships:

- Route: Each Subroute is associated with one Route.
## Refund
### Attributes:

- refundId: Unique identifier for the refund.
- paymentId: The payment associated with this refund.
- amount: Amount of the refund.
- refundDate: Date and time when the refund was processed.
- reason: Reason for the refund.
- status: Status of the refund (e.g., Processed, Pending).
### Relationships:

- Payment: Each Refund is related to one Payment (i.e., a refund is made for a specific payment).
- Transaction: Each Refund is linked to one or more Transactions (a refund could affect multiple transactions or be part of transaction records).
## Feedback
### Attributes:

- feedbackId: Unique identifier for the feedback.
- userId: The user who provided the feedback.
- orderId: The order related to the feedback.
- rating: Rating given by the user.
- comments: Comments or additional information provided by the user.
- timestamp: Date and time when the feedback was submitted.
### Relationships:

- User: Each Feedback is associated with one User.
- Order: Each Feedback is associated with one Order.
