# Selection of a Software Process Model
The lab requires us to identify a process model, justify it, identify its overheads/drawbacks, and explain how we will manage them.

## Selected Process Model: Incremental Model
I recommend the Incremental Model.

### Justification
The Incremental Model is appropriate for the La Roche Pharmacy system because the project contains several related but separable functions. Instead of attempting to develop the entire pharmacy system at once, the development team can divide it into smaller increments.
For example:

#### Increment 1 — Core Website and Accounts
* Pharmacy homepage
* Medicine/product browsing
* Search functionality
* Customer registration/login
* Customer profile

#### Increment 2 — Online Ordering
* Shopping cart
* Checkout
* Order creation
* Payment process
* Order history

#### Increment 3 — Prescription Processing
* Prescription upload
* Prescription review
* Pharmacist approval/rejection
* Linking approved prescriptions to orders
* Customer notification

#### Increment 4 — Pharmacy Operations
* Staff dashboard
* Order preparation
* Inventory management
* Medicine availability
* Order-status updates

#### Increment 5 — Owner/Administration
* Staff account management
* Role/access management
* Product management
* Pricing management
* Reports and system monitoring

This follows the lecture's description of developing the core product first and then adding further functionality through successive increments.

Another advantage is that the team can produce a working version early and receive feedback before completing the entire project. This is particularly useful because some pharmacy workflows, such as prescription approval and staff permissions, may need refinement as the team better understands the pharmacy's actual procedures.

### Major overheads and drawbacks
One drawback mentioned in the lecture is that the Incremental Model can require significant planning and that integration between different increments can become complicated, increasing development time and cost.

For our project, possible issues include:
* Integrating prescription processing with the ordering system.
* Ensuring inventory is updated correctly after an order.
* Maintaining consistent user authentication across all increments.
* Ensuring staff and owner permissions remain consistent.
* Avoiding database structure changes that break earlier increments.
* Coordinating work between team members.

#### Strategy for managing these drawbacks
The team will define the overall architecture, main database entities, user roles, and interfaces before implementing individual increments. GitHub will be used for version control and collaboration.

We will also establish common components such as authentication, medicine information, users, and order identifiers early in development so later increments can reuse them.

Each increment will be individually tested before integration with the existing system. The team will also maintain clear documentation to reduce inconsistencies between increments.