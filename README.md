# airbnb-clone-project
ALX  Pro-dev backend development AirBnb clone Project.

# Team Roles
1. Business Analyst
    -Understands customer's business processes and translates customer business needs into requirements.

2. Product Owner
    -Holds responsibility for a product vision and evolution and make sure the final prduct meets customer requirements.

3. Project Manager
    -Make sure a product or its part is delivered on time and within budget.
    -They also manage and motivate the software development team.

4. UI/UX Designer
    -Transforms a product vision into user-friendly designs.
    -Creates user journeys for the best use experience and highest conversion rates.

5. Software Architect
    -Designs a high-level software architecture.
    -Selects appropriate tools and platform to implement the product vision.
    -Sets up code quality standards and performs code reviews.

6. Software Developer
    -Engineers and stabilizzes the product.
    -Solvees any techinical pronlems emerging during the development life cycle.

7. Quality Assurance Engineer
    -Makes sure an application performs according to requirements.
    -Spots functional and non-functional defects.

8. Test Automation Engineer
    -Designs a test automation ecosystem.
    -Writes and maintains test scripts for auomated testing.

9. DevOps Engineer
    -Facilitates a cooperation between development and operations teams.
    -Builds continuous integration and continuous delivery (CI/CD) pipelines for faster delivery.

# Technology Stack

1. Django
    -Povides a comprehensive RESTful API for handling CRUD operations on user and property data.

2. GrapghQL
    -Offers a fleible and efficient query mechanism for interacting with the backend.

3. PostgreSQL
    -A powerful relational database used for data storage.

4. Celery
    -For handling asynchronous tasks such as sending notifications or processing payments.

5. Django REST Framework
    -Povide tools for creating and managing RESTful APIs.

6. Redis
    -Used for caching and session management.

7. Docker
    -Containeriization tool for consistent development and deployment environments.

8. CI/CD Pipelines
    -Automated pipelines for testing and deploying code changes.

# Database Design
1. Entities required
    -Users
        a. Properties- One user can occupy multiple properties.
        b. Bookings- One user can have multiple bookings.
        c. Reviews- One user can make multiple review.
        d. Payments- One user can make multiple payments.
    
    -Properties
        a. Users- One property can only be occupied by one user.
        b. Bookings- One property can have one booking.
        c. Reviews- One property can be reviewed by many users.
        d. Payments- One property can be paid for multiple times.
    
    -Bookings
        a. Users- One booking can be made by one user.
        b. Properties- One booking can be made on one property.
        c. Payments- One booking can have multiple payment instances.

    -Reviews
        a. Users - One review can only be made by one user.
        b. Properties- One review can be made on one property.
    
    -Payments
        a. Users- One payment instance can be made by one user.
        b. Bookings- One payment nstance can be made for multiple bookings.
