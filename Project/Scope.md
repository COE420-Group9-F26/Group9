# Project Scope

The lab requires the project scope to contain the project objective, target users, in-scope features, out-of-scope features, and major deliverables.

## 1. Project Objective
The objective of the La Roche Pharmacy Online Prescription and Medicine Management System is to develop a web-based system that allows customers to interact with the pharmacy digitally while allowing pharmacy staff and management to efficiently process and manage online pharmacy operations.

The system aims to provide customers with a convenient method for browsing pharmacy products, submitting prescriptions, purchasing medicines and other products, making payments, and tracking orders.

For pharmacy staff, the system will provide tools for reviewing prescriptions, managing customer orders, checking medicine availability, preparing orders, updating order status, and maintaining inventory information.

For the pharmacy owner, the system will provide administrative control over staff accounts, products, prices, inventory, orders, and other important pharmacy information.

## 2. Target Users

### Customers
Customers are people using the pharmacy website to:
* Register and log in.
* Browse medicines and pharmacy products.
* Search for products.
* View product information.
* Upload prescriptions.
* Add products to a cart.
* Purchase products online.
* Track existing orders.
* View previous orders.
* Manage their profile.

### Pharmacy Staff / Pharmacists
Staff members are responsible for operational pharmacy processes. Depending on their permissions, they can:
* Log in to the staff portal.
* View incoming orders.
* Review uploaded prescriptions.
* Approve or reject prescriptions.
* Check medicine availability.
* Prepare orders.
* Update order status.
* Update inventory quantities.
* Contact customers regarding an order or prescription.

### Pharmacy Owner / Administrator
The owner has the highest level of access and can:
* Monitor pharmacy operations.
* Add, edit, or remove medicines/products.
* Update medicine prices.
* Manage inventory.
* Create and manage staff accounts.
* Assign staff roles and permissions.
* View all orders.
* View reports/statistics.
* Manage website information.

## 3. In-Scope Features

### Customer Account Management
* Customer registration.
* Customer login/logout.
* Customer profile.
* Password management.
* Address/contact information.
* Order history.

### Medicine and Product Catalogue
* Display medicines and pharmacy products.
* Product name.
* Product description.
* Product image.
* Price.
* Availability.
* Product category.
* Search.
* Filtering.

### Online Shopping Cart
* Add products.
* Remove products.
* Change quantities.
* Display total cost.
* Proceed to checkout.

### Prescription Upload
Customers can upload a prescription when purchasing products requiring pharmacist verification.

### Prescription Review
Authorized pharmacy staff can:
* View the uploaded prescription.
* Review the prescription.
* Approve the prescription.
* Reject the prescription.
* Request clarification when necessary.

### Order Management
The system will have the following ideal workflow:

**Pending → Prescription Review → Approved → Payment/Confirmed → Preparing → Ready/Out for Delivery → Completed**

Alternative/error states can include:

* Prescription Rejected
* Cancelled
* Payment Failed

### Online Payment
Customers can proceed through a payment process as part of checkout.

For the course prototype, payment can be represented using a test/simulated payment gateway rather than processing actual financial transactions.

### Inventory Management
Authorized staff can:
* View stock.
* Update quantities.
* Identify unavailable medicines.
* Reduce inventory when orders are processed.

### Staff Management
The owner can:
* Add staff.
* Remove/deactivate staff.
* Modify staff details.
* Assign roles.
* Assign permissions.

### Role-Based Access Control
At minimum we will have:

| Role          | Main Access                                     |
| :---          | :---                                            |
| Customer      | Shopping, prescriptions, checkout, orders       |
|Pharmacy Staff | Orders, prescriptions, inventory                |
|Pharmacist     | Prescription verification + staff functionality |
|Owner/Admin    | Complete administrative control                 |

This is an important design decision because different users should not have equal access to sensitive functions.

### Product Management
Owner/authorized staff can:
* Add products.
* Edit products.
* Update prices.
* Update descriptions.
* Update quantities.
* Mark products available/unavailable.

### Order Tracking
Customers can see the current status of their orders.

### Notifications
Basic notifications can inform customers when:
* Prescription is accepted.
* Prescription is rejected.
* Payment succeeds/fails.
* Order is being prepared.
* Order is ready.
* Order is completed.

## 4. Out-of-Scope Features
To prevent the project from becoming too large for the semester, the initial version will not include:
* Integration with real hospitals or government health databases.
* Automatic verification of prescriptions using external medical systems.
* Automatic diagnosis.
* Medical advice generated by the software.
* Telemedicine consultations.
* Real insurance-claim processing.
* Real banking/payment production infrastructure.
* Automated medicine dispensing robots.
* Multiple pharmacy branches with complex cross-branch logistics.
* Real-time GPS delivery-driver tracking.
* Integration with pharmacy suppliers for automatic purchasing.
* AI-based medicine recommendations.
* Native Android/iOS applications.

These features may be considered future extensions.

This is important because the lecture stresses defining system boundaries: what is inside and outside the system.

## 5. Major Deliverables
* The project's expected deliverables include:
* Customer interface.
* Pharmacy staff interface.
* Owner/administrator interface.
* Product catalogue.
* Customer account system.
* Shopping-cart system.
* Prescription submission system.
* Prescription review system.
* Order-management system.
* Inventory-management system.
* Role-based access-control system.
* Database.
* System documentation.
* Software requirements documentation.
* UML diagrams.
* System design documentation.
* Source code.
* Test cases and testing documentation.
* GitHub repository.
* Final project report.