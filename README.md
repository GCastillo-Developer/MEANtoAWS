Overview
-------------------------------------------------------------------------------------------------------------------------------------------------
This project documents the migration of the original MEAN stack TRAVLR application into a cloud‑native microservices architecture on AWS.
The migration focused on modernizing the application for scalability, maintainability, and operational efficiency using:

• Docker containerization
• AWS serverless services (S3, Lambda, DynamoDB)
• Cloud‑native design principles
• Security best practices
• Infrastructure decoupling and modularization

To demonstrate the architecture, decisions, and lessons learned, I also recorded a presentation walkthrough explaining the migration process and key cloud concepts.

Key Features
• Dockerized Services  
• Containerized the application components for portability and consistent deployment.

AWS Lambda Functions  
• Offloaded backend logic into serverless compute for cost‑efficient execution.

Amazon S3  
• Used for static asset hosting and durable storage.

DynamoDB  
• Implemented a NoSQL database layer to replace or complement MongoDB.

API Gateway  
• Managed routing, authentication, and request handling for serverless endpoints.

Security Enhancements  
• Applied IAM roles, least‑privilege access, environment variable protection, and secure API design.

Cloud‑Native Architecture  
• Broke the monolithic MEAN app into modular, independently deployable components.

Original Architecture (Before Migration)
The original TRAVLR app was built using the MEAN stack:
• MongoDB for data persistence
• Express.js for backend routing
• Angular for the admin UI
• Node.js for server logic
• Handlebars for server‑side rendering
• CSS + JavaScript for styling and interactivity

This monolithic structure was then re‑engineered for AWS.

Cloud‑Native Architecture (After Migration)
Core AWS Components
• AWS Lambda — Stateless compute for backend logic
• Amazon S3 — Static hosting + file storage
• DynamoDB — NoSQL database
• API Gateway — Routing + API management
• IAM — Secure access control
• CloudWatch — Logging + monitoring

Modernization Goals
• Reduce operational overhead

Improve scalability
• Increase fault tolerance
• Lower cost through serverless compute
• Decouple services for easier maintenance
