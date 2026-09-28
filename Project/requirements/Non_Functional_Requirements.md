# Non-Functional Requirements

## Individual Contributions

### Alan Dsouza

NFR-A1

The system should adhere to confidentiality standards such as HIPAA.

NFR-A2

The system should be easily adaptable to various pharmacies.

NFR-A3

The system should be easily upgraded or maintained remotely.

NFR-A4

The system's inventory tracking system should support all relevant attributes for any medication and support the variety that would be stocked at any reasonable pharmacy.

NFR-A5

The system should maintain role-based access reliably without customers being able to access the pharmacist UI without appropriate credentials.


### Omar Alkhatib

NFR-OA1

The system should store user passwords using secure one-way hashing and shall never store them as plain text.

NFR-OA2

The system should maintain an audit log of prescription approvals and rejections, including the responsible pharmacist and the date and time of the action.

NFR-OA3

The system should preserve data consistency so that interrupted payments or order-processing errors do not create duplicate orders or incorrect inventory updates.

NFR-OA4

The system should provide a clear user-friendly interface for customers and pharmacy staff.

NFR-OA5

The system should protect customers' personal and prescription information from unauthorized access.


### Qusai Al Tah

NFR-Q1

The system should display the prescription review page within 3 seconds for at least 95% of requests under normal operating conditions.

NFR-Q2

The system shall complete at least 95% of medicine search requests within 2 seconds under normal operating conditions.

NFR-Q3

The system shall maintain at least 99% availability during the pharmacy's normal operating hours, excluding scheduled maintenance.

NFR-Q4

The system shall use encrypted HTTPS communication for all customer, prescription, payment, and account data transmitted between the user and the server.

NFR-Q5

The customer interface shall support responsive layouts for desktop, tablet, and mobile screen sizes without loss of core functionality.


### Omar Abdalla

NFR-OD1

When a prescription upload fails, the system should display a clear error message identifying the reason for the failure and allow the customer to retry the upload without restarting the checkout process.

NFR-OD2

The system should automatically end an authenticated customer session after 20 minutes of inactivity and require the user to log in again.

NFR-OD3

The system should support the latest versions of Google Chrome, Microsoft Edge, and Mozilla Firefox without requiring browser-specific installation or configuration.

NFR-OD4

The system should preserve confirmed customer orders in persistent storage so that the order remains available after the customer logs out and later logs back in.

NFR-OD5

The system should require confirmation from the customer before permanently cancelling an eligible order.


# Team Consolidated Non-Functional Requirements

The team reviewed all Non-Functional Requirements before consolidation. No requirements were removed or merged because no duplicate requirements were identified.

NFR-01

The system should adhere to confidentiality standards such as HIPAA.

NFR-02

The system should be easily adaptable to various pharmacies.

NFR-03

The system should be easily upgraded or maintained remotely.

NFR-04

The system's inventory tracking system should support all relevant attributes for medications and the range of products expected in a pharmacy.

NFR-05

The system should reliably maintain role-based access and prevent unauthorized access to restricted interfaces.

NFR-06

The system should store user passwords using secure one-way hashing and shall never store passwords as plain text.

NFR-07

The system should maintain an audit log of prescription approvals and rejections, including the pharmacist and date and time of the action.

NFR-08

The system should preserve data consistency so interrupted payments or order-processing errors do not create duplicate orders or incorrect inventory updates.

NFR-09

The system should provide a clear user-friendly interface for customers and pharmacy staff.

NFR-10

The system should protect customers' personal and prescription information from unauthorized access.

NFR-11

The system should display the prescription review page within 3 seconds for at least 95% of requests under normal operating conditions.

NFR-12

The system shall complete at least 95% of medicine search requests within 2 seconds under normal operating conditions.

NFR-13

The system shall maintain at least 99% availability during the pharmacy's normal operating hours, excluding scheduled maintenance.

NFR-14

The system shall use encrypted HTTPS communication for all customer, prescription, payment, and account data transmitted between the user and the server.

NFR-15

The customer interface shall support responsive layouts for desktop, tablet, and mobile screen sizes without loss of core functionality.

NFR-16

When a prescription upload fails, the system should display a clear error message identifying the reason and allow the customer to retry without restarting the checkout process.

NFR-17

The system should automatically end an authenticated customer session after 20 minutes of inactivity and require the user to log in again.

NFR-18

The system should support the latest versions of Google Chrome, Microsoft Edge, and Mozilla Firefox without requiring browser-specific installation.

NFR-19

The system should preserve confirmed customer orders in persistent storage so orders remain available after the customer logs out and logs back in.

NFR-20

The system should require confirmation from the customer before permanently cancelling an eligible order.
