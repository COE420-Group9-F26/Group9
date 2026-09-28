# Use Cases

## Individual Contributions

### Alan Dsouza

UC-A1 - Submit Prescription

Primary Actor: Customer

The customer submits a prescription they received from their doctor or practitioner.

UC-A2 - Cancel Order by Pharmacist

Primary Actor: Pharmacist

The pharmacist cancels an order due to inventory problems or other issues where they are unable to fulfill it.

UC-A3 - Complete Payment

Primary Actor: Customer

The customer enters their payment information and pays for a prescription after it has been approved and before it will be fulfilled.

UC-A4 - Add Medication

Primary Actor: Pharmacy Admin

The pharmacy administrator adds a new medication to the inventory and fills in its attributes and available stock.

UC-A5 - Edit Medication

Primary Actor: Pharmacy Admin

The pharmacy administrator edits an existing medication's attributes or availability.


### Omar Alkhatib

UC-OA1 - View Prescription Status

Primary Actor: Customer

The customer views the current status of their submitted prescription.

UC-OA2 - Receive Prescription Status Notification

Primary Actor: Customer

The customer receives a notification when the pharmacy updates the prescription status.

UC-OA3 - Delete Medication

Primary Actor: Pharmacy Admin

The pharmacy administrator removes a discontinued or permanently unavailable medication from the product catalogue.

UC-OA4 - Request Prescription Clarification

Primary Actor: Pharmacist

The pharmacist requests additional information from a customer when an uploaded prescription is unclear or incomplete.

UC-OA5 - Retry Failed Payment

Primary Actor: Customer

After a payment attempt fails, the customer retries the payment using the same or a different payment method.


### Omar Abdalla

UC-OD1 - Approve Prescription

Primary Actor: Pharmacist

After reviewing a valid prescription, the pharmacist approves it and the system records its status as approved so the associated order may continue.

UC-OD2 - Reject Prescription

Primary Actor: Pharmacist

After reviewing an invalid prescription, the pharmacist rejects it and the system records its status as rejected, preventing the associated order from proceeding to payment.

UC-OD3 - Cancel Order

Primary Actor: Customer

The customer selects an eligible order that has not yet entered preparation and requests cancellation. The system updates the order status to cancelled.

UC-OD4 - View Order History

Primary Actor: Customer

The customer views a list of previously placed orders, including the order date, total amount, and final status.

UC-OD5 - Manage Shopping Cart

Primary Actor: Customer

The customer changes item quantities or removes products from the shopping cart before proceeding to checkout.


### Qusai Al Tah

UC-Q1 - Search for Medicine

Primary Actor: Customer

The customer searches for a medicine using its name, category, or active ingredient and views matching products.

UC-Q2 - View Medicine Details

Primary Actor: Customer

The customer selects a medicine and views its price, availability, description, and whether a prescription is required.

UC-Q3 - Select Fulfillment Method

Primary Actor: Customer

The customer chooses either pharmacy pickup or delivery when completing an order.

UC-Q4 - Update Order Preparation Status

Primary Actor: Pharmacy Staff

An authorized pharmacy staff member updates the status of an order as it moves through preparation.

UC-Q5 - Receive Order Ready or Dispatch Notification

Primary Actor: Customer

The customer receives a notification when the order becomes ready for pickup or is dispatched for delivery.


# Team Consolidated Use Cases

The team reviewed all twenty individual Use Cases. None of the original Use Cases were removed or merged. All twenty were retained.

During the consistency review, four additional team-level Use Cases were added because corresponding functionality was present in the Functional Requirements but was not represented clearly as a Use Case.

UC-01 - Submit Prescription

UC-02 - Cancel Order by Pharmacist

UC-03 - Complete Payment

UC-04 - Add Medication

UC-05 - Edit Medication

UC-06 - View Prescription Status

UC-07 - Receive Prescription Status Notification

UC-08 - Delete Medication

UC-09 - Request Prescription Clarification

UC-10 - Retry Failed Payment

UC-11 - Approve Prescription

UC-12 - Reject Prescription

UC-13 - Cancel Order

UC-14 - View Order History

UC-15 - Manage Shopping Cart

UC-16 - Search for Medicine

UC-17 - View Medicine Details

UC-18 - Select Fulfillment Method

UC-19 - Update Order Preparation Status

UC-20 - Receive Order Ready or Dispatch Notification


## Additional Team Use Cases

UC-21 - Register Account

Primary Actor: Customer

The customer creates a new account by providing the required registration information.

UC-22 - Log In

Primary Actors: Customer, Pharmacist, Pharmacy Staff, Pharmacy Admin, Pharmacy Owner

A registered user enters valid credentials and receives access to the system according to their assigned role.

UC-23 - Manage Staff Accounts

Primary Actor: Pharmacy Owner

The pharmacy owner creates, updates, deactivates, and assigns roles to staff accounts.

UC-24 - Review Prescription

Primary Actor: Pharmacist

The pharmacist opens and reviews a submitted prescription before deciding whether to approve it, reject it, or request clarification.


# Use Case Relationships

The team reviewed the final Use Cases to identify appropriate <<include>> and <<extend>> relationships.

The <<extend>> relationship is used when additional behavior occurs only under a particular condition or is optional.

The <<include>> relationship is used when one Use Case must always perform another Use Case as part of its behavior.

The team did not identify a necessary <<include>> relationship among the current Use Cases. Therefore, an artificial <<include>> relationship was not added simply to satisfy the diagram.

## R-01

Base Use Case: Complete Payment

Related Use Case: Retry Failed Payment

Relationship: <<extend>>

Justification: Retry Failed Payment only occurs when the original payment attempt fails. If payment succeeds, this additional behavior is not required.

## R-02

Base Use Case: Review Prescription

Related Use Case: Request Prescription Clarification

Relationship: <<extend>>

Justification: Request Prescription Clarification occurs only when the pharmacist determines that the submitted prescription is unclear or incomplete.

## R-03

Base Use Case: Review Prescription

Related Use Case: Approve Prescription

Relationship: <<extend>>

Justification: Approve Prescription occurs when the pharmacist determines that the reviewed prescription is valid.

## R-04

Base Use Case: Review Prescription

Related Use Case: Reject Prescription

Relationship: <<extend>>

Justification: Reject Prescription occurs when the pharmacist determines that the reviewed prescription is invalid.

## R-05

Base Use Case: Search for Medicine

Related Use Case: View Medicine Details

Relationship: <<extend>>

Justification: After searching for a medicine, the customer may select one of the search results to view additional information.

## R-06

Base Use Case: Update Order Preparation Status

Related Use Case: Receive Order Ready or Dispatch Notification

Relationship: <<extend>>

Justification: The notification is triggered only when the updated order status becomes ready for pickup or dispatched for delivery.
