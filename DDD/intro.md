## What is the purpose of DDD?
$ For business people and developers to collaborate effectively
$ To understand the context of the problem
## What is Domain?
$ A "set" of activities and processes
$ A "field" in which "business operates"
``` 
People will be successful at DDD if they understand the domain they need to model.
```
$ Domain is composed of several different activities
## What is subdomain?
$ Subdomain is a peace (part) of domain. Subdomains are results of breaking whole domain into peaces to understand it easily<br>
$ A subdomain is a subpart of the big domain model, which operates through its own business logic and processes.
$ A subdomain can also become a domain. It depends on the level of focus given to the analysis of a domain. If we analyze a subdomain with more focus and divide it into its own sub activities, it can also become a domain. <br>
$ Subdomains have 3 categories:
 - Core domain - main activities that make up business, activities and processes that make business unique and stand out from other businesses in the field: product recommendation, source management
 - Supporting domain - processes or activities that support the smooth operation of core domain activities: Product stock management
 - Generic domain - processes or activities not specific to domain but common in many businesses: account management, authorization, human resources, payroll.

**Core domain**
```
- Book Catalog Management: Creating, organizing, and maintaining a detailed catalog of books that customers can browse and purchase. This includes metadata like authors, genres, pricing, availability, and customer reviews.
- Book Recommendation System: Developing algorithms that recommend books to customers based on their past purchases, browsing history, or ratings. This is a key differentiator that can increase sales and improve customer satisfaction.
- Order Processing: Handling customer orders from the moment they are placed until the books are delivered. This includes selecting the correct books, processing payments, and managing order fulfillment.
```
**Supporting domain**
```
1. E-commerce Platform
* Supporting Subdomain: Logistics and Shipping Management
Explanation: For an e-commerce platform like Amazon, the core domain might be the product catalog and order processing. However, the logistics and shipping management subdomain, which involves coordinating with shipping carriers, managing warehouses, and tracking deliveries, is crucial for getting products to customers. While essential, it's not the primary differentiator for the platform—customers expect their orders to arrive on time, but the logistics process itself isn’t what makes the platform unique.
2. Healthcare System
* Supporting Subdomain: Patient Scheduling
Explanation: In a healthcare system, the core domain could involve diagnosis and treatment of patients. A supporting subdomain like patient scheduling is essential for the smooth operation of the healthcare facility, ensuring that doctors' time is effectively managed and patients are seen promptly. However, the scheduling system itself doesn’t provide direct patient care; it supports the core activities of medical treatment.
3. Online Education Platform
* Supporting Subdomain: Course Material Management
Explanation: The core domain for an online education platform might be the creation and delivery of educational content. A supporting subdomain like course material management involves organizing, updating, and distributing the course materials to students. This is critical for the functioning of the platform but is not the key value proposition—students enroll for the educational experience, not necessarily for how well the materials are managed.
4. Banking System
* Supporting Subdomain: Fraud Detection and Prevention
Explanation: In a banking system, the core domain might involve managing customer accounts, transactions, and loans. A supporting subdomain like fraud detection and prevention is crucial for protecting the bank and its customers from fraudulent activities. Although this function is vital, it’s considered a supporting subdomain because the bank’s core business revolves around financial services, not necessarily the detection of fraud.
5. Retail Business
* Supporting Subdomain: Inventory Replenishment
Explanation: In a retail business, the core domain might be sales and customer service. Inventory replenishment, which involves ensuring that products are restocked efficiently to meet customer demand, is a supporting subdomain. While it’s essential to keep the business running smoothly, it supports the core activities of selling products and providing customer service rather than defining the business's competitive edge.
6. Social Media Platform
* Supporting Subdomain: Content Moderation
Explanation: For a social media platform like Facebook, the core domain could be connecting users and facilitating social interactions. Content moderation, which involves reviewing and managing user-generated content to ensure it meets community guidelines, is a supporting subdomain. This function is vital for maintaining the platform’s integrity but is not the core reason users engage with the platform.
7. Manufacturing Company
* Supporting Subdomain: Equipment Maintenance
Explanation: In a manufacturing company, the core domain might involve the design and production of goods. A supporting subdomain like equipment maintenance ensures that machinery and production lines are operational and efficient. While crucial to preventing downtime, equipment maintenance supports the primary production activities rather than being the core focus of the business.

Summary:

- E-commerce Platform: Logistics and Shipping Management supports order fulfillment but isn't what makes the platform unique.

- Healthcare System: Patient Scheduling ensures smooth operations but doesn’t directly involve patient care.

- Online Education Platform: Course Material Management organizes resources but isn’t the core educational service.

- Banking System: Fraud Detection and Prevention protects the system but isn’t the main financial service offered.

- Retail Business: Inventory Replenishment keeps products in stock but isn’t the main selling point.

- Social Media Platform: Content Moderation maintains platform integrity but doesn’t create social connections.

- Manufacturing Company: Equipment Maintenance keeps production running smoothly but isn’t the core production activity.

-These examples should give you a clearer understanding of what constitutes a supporting subdomain across various domains
```
**Generic domains**
```
1. E-commerce Platform
Generic Subdomain: User Authentication
Explanation: For an e-commerce platform like Amazon, user authentication (managing user logins, passwords, and access control) is a necessary function that is common to almost any online service. It ensures that only authorized users can access their accounts and make purchases. However, this function is not unique to e-commerce; it’s a standard requirement for most web applications.
2. Healthcare System
Generic Subdomain: Payroll Management
Explanation: In a healthcare system, payroll management is essential for ensuring that doctors, nurses, and other staff are paid correctly and on time. While critical to the operation of the healthcare facility, payroll management is not specific to healthcare—it’s a function that exists in virtually every organization, regardless of industry.
3. Online Education Platform
Generic Subdomain: Customer Support Ticketing
Explanation: An online education platform needs to handle customer support requests, which might involve issues with accessing course materials or technical problems. A customer support ticketing system allows users to submit requests and track their resolution. This system is common across many industries and does not specifically relate to the educational content or services offered by the platform.
4. Banking System
Generic Subdomain: Document Management
Explanation: In a banking system, managing various documents (such as contracts, account statements, and loan applications) is necessary for compliance and operational purposes. Document management is a generic subdomain because it involves storing, organizing, and retrieving documents, which is a requirement in many different industries, not just banking.
5. Retail Business
Generic Subdomain: Email Marketing
Explanation: For a retail business, email marketing campaigns are used to communicate with customers, promote products, and increase sales. However, email marketing is a generic function that many businesses use across various domains to engage with their customers, making it a generic subdomain rather than something unique to retail.
6. Social Media Platform
Generic Subdomain: Data Backup and Recovery
Explanation: A social media platform must ensure that user data is backed up and can be recovered in case of a system failure or data loss. Data backup and recovery is a generic subdomain because it is a standard practice in any business that handles digital information, not something unique to social media platforms.
7. Manufacturing Company
Generic Subdomain: Human Resources Management
Explanation: In a manufacturing company, managing employees—recruiting, training, performance evaluations, and benefits administration—is essential. However, human resources management is a generic subdomain because it is required in nearly every business, regardless of the industry.
Summary:
E-commerce Platform: User Authentication is common to any online service, not unique to e-commerce.
Healthcare System: Payroll Management is a standard business function, not specific to healthcare.
Online Education Platform: Customer Support Ticketing is a common feature across industries.
Banking System: Document Management is required in many sectors, not just banking.
Retail Business: Email Marketing is a typical business activity across various domains.
Social Media Platform: Data Backup and Recovery is standard for any digital platform.
Manufacturing Company: Human Resources Management is a common need in all businesses.
These examples highlight how generic subdomains are essential yet not unique to a specific business domain. They are functions that any business, regardless of industry, would need to manage effectively.
```
A person can learn different domains but can be an expert in one

## Domain-Driven Design
```
Domain Driven Design aims to develop any complex software based on understanding a business with its processes and representing such processes in something called a model.
```
```
DDD is the design to solve complex problems faced when building business with big domain. In DDD we structure how our models are organized and interact with each other. It helps us from tactical, technological and strategical perspectives. 
```
```
DDD is for complex domains only
```
- The most important aspect of DDD is modeling a domain and subdomains, not defining the technology stack or something related to technology
- Breaking domain into subdomains: After modeling domain, team should break it into subdomains, analyze and clearly understand the subdomains, and build the business model which will represent business processes
- MVP is best for DDD: Team should create a basic model that is easy to understand first. The model should be easy for others to evolve sprint by sprint till its ultimate state. 

DDD concepts that define it(its rules) are: 
- Entity
- Value Object
- Aggregate
- Domain Event
- Command
- Query
- Service
- Repository
- Factory

**Strategic approach**<br>
Modeling domain and structuring the entire process of it.<br>
It helps us during modeling the domain. Provides(uses) patterns like bounded context and ubiquitous language to solve problems and achieve goals set by DDD. It is the GENERAL way of solving the problem. It applies to every piece of the model and subdomains. We draw diagrams that show the flow of activities

**Tactical approach**<br>

Used when translating a model into a specific piece of software. When writing code that implements the logic of the model
This approach solve problems that arise during the development process of software.

In DDD the approches are: 

- MVP
- Strategic approach
- Tactical approach

## Pros and Cons of DDD

**Pros**

- Flexibility. Easy to evolve business logic(process), software that is implemented and technologies used.
- Organized code. DDD can work with hexagonal architecture. This architecture gives us specific structure of our code. This way we will have the code that is easy to modify.
- Business logic is not spread across application code. In hexagonal architecture, we have a layer which stores all the business logic and objects. Because of this separation, we can easily modify our business logic as we need to focus on it only. 
- Easy communication between business people and development team. To achieve it the code should use business language terminology
- Domain is more important that UI/UX. This point highlights a key strength of Domain-Driven Design (DDD): its focus on the underlying business logic and domain, rather than the superficial aspects like the user interface (UI) or user experience (UX). Here's a breakdown of what this means and why it's considered an advantage:

  1. Focus on Core Business Logic
     In DDD, the primary concern is understanding and accurately modeling the domain—the real-world problem or business area the software is intended to address. This means that the technical team prioritizes building a robust, well-structured domain model that encapsulates the core business rules, processes, and concepts.

    Why It's Important: The domain is the essence of the business, representing its unique value and competitive advantage. By focusing on the domain, the software can truly support and enhance the business, solving the right problems and delivering real value.
  2. Separation of Concerns
     In DDD, there's a clear separation between the domain layer (where business logic resides) and other layers like the application layer (which coordinates tasks) and the presentation layer (UI/UX). This separation ensures that the core business logic remains isolated and unaffected by changes in the UI or UX.

    Why It's Important: UI/UX trends can change rapidly, and software might need to adapt to new interfaces (e.g., from web to mobile). If the business logic is tightly coupled with the UI, making these changes can become costly and error-prone. DDD’s approach allows the UI to be modified or even completely replaced without impacting the core domain logic.
  3. Longevity and Maintainability
     Because DDD emphasizes a strong, well-designed domain model, the software tends to be more maintainable and adaptable over time. The domain model is not as likely to become obsolete because it's based on the enduring aspects of the business, rather than transient UI/UX trends.

    Why It's Important: Software that remains relevant and easy to maintain over the long term reduces costs and increases the return on investment. Businesses can evolve their interfaces or add new features without having to rewrite the core logic.
  4. True Business Alignment
     By focusing on the domain, DDD ensures that the software is closely aligned with the business’s needs. The domain model acts as a direct reflection of the business processes, terminology, and rules. This alignment is more critical to the business's success than having a visually appealing interface, especially in complex or highly specialized industries.

    Why It's Important: Misalignment between the software and the business domain can lead to inefficiencies, errors, and missed opportunities. DDD minimizes this risk by ensuring that the software’s backbone—the domain model—faithfully represents the business.
  5. Flexibility in UI/UX
     Since the domain is separate from the UI/UX, different interfaces can be built on top of the same domain model. For example, you could have a web interface, a mobile app, and an API all interacting with the same underlying domain logic.

    Why It's Important: This flexibility allows businesses to offer multiple ways to interact with the software, catering to different user needs and devices without having to duplicate or significantly alter the core logic.<br>
**Conclusion**<br>
The statement emphasizes that in DDD, the true value of the software lies in its domain model, not in its appearance or how users interact with it. While UI/UX are important for user satisfaction, they are considered secondary to getting the business logic right. This focus on the domain ensures that the software is aligned with the business’s goals, adaptable over time, and maintainable in the long run, providing a strong foundation that can support various user interfaces as needed.
This is one of the key reasons why DDD is favored in complex and mission-critical systems where the domain is the most crucial aspect of the business.