# Build a Fullstack Inventory Management Dashboard

Click the link below to watch the presentation recording

[![Presentation Video](server\assets\webpage.png)](https://unomail-my.sharepoint.com/personal/aamoussou_unomaha_edu/_layouts/15/stream.aspx?id=%2Fpersonal%2Faamoussou%5Funomaha%5Fedu%2FDocuments%2FRecordings%2FCSCI4650%20%2D%20Group%204%2D20241205%5F204217%2DMeeting%20Recording%2Emp4&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E94915a08%2D42ee%2D4ac9%2Dbcf5%2Dacfbf73f13ee)


# Overview

An advanced, feature-rich Inventory Management Web Application built with a modern tech stack to manage, organize, and monitor inventory efficiently. This application leverages Next.js for the frontend and Node.js for the backend, with seamless integrations for storage, APIs, and cloud hosting.

# Features

- Inventory Tracking: Manage and track inventory in real time.
- Data Grid Integration: Intuitive data table for efficient inventory visualization and manipulation.
- API Integration: High-performance APIs for CRUD operations using AWS API Gateway.
- Cloud Hosting: Scalable backend and database hosted on AWS EC2 and AWS RDS.
- File Uploads: Upload inventory-related documents and images using AWS S3.

# Tech Stack

## FrontEnd
- next.js: React-based framework for server-side rendering and static site generation.     
- Tailwind CSS: Utility-first CSS framework for rapid UI development.     
- Redux Toolkit: State management with simplified configurations.     
- Redux Toolkit Query (RTK Query): Efficient data fetching and caching.     
- Material UI Data Grid: Feature-packed, customizable data grid for data visualization.

## BackEnd
- node.js: Backend runtime for building APIs and server logic.     
- Prisma: Modern ORM for database schema and queries.

## CloudServices

- AWS EC2: Hosting scalable backend services. 
- AWS MySQL: Used to store and retrieve data for our application.    
- AWS RDS: Managed relational database service for reliable database hosting.     
- AWS API Gateway: Managed API layer for secure and scalable API calls.     
- AWS Amplify: Simplifies the hosting and deployment of frontend assets.     
- AWS S3: Cloud storage for file uploads and static assets. 


# Setup Instructions

## Prerequisites

- Node.js (>=16.0.0)     
- PostgreSQL Database (or AWS RDS instance)     
- AWS Account for cloud services     
- Prisma CLI : npm install -g prisma

## Installation

- Clone the repository: git clone https://github.com/benjaakpe/inventory-tracking-app.git 
- cd Term-Project-Group-4Install 
- dependencies: npm install
- Set up the environment variables
- Create .env files for both the server and frontend
- Server ".env":
- DATABASE_URL=postgresql://username:password@aws-rds-endpoint:5432/database_name
- AWS_ACCESS_KEY_ID=your-access-key
- AWS_SECRET_ACCESS_KEY=your-secret-key
- AWS_REGION=your-region
- Client ".env.local":
- NEXT_PUBLIC_API_BASE_URL=https://your-api-gateway-endpoint
- Initialize Prisma: prisma migrate dev --name init
- Start the development server: npm run dev

## Deployment

### Frontend     
- Deploy the Next.js frontend using AWS Amplify hosting service:         
    - amplify init         
    - amplify publish     
    
### Backend:         
- Deploy the backend to an AWS EC2 instance.         
- Use AWS API Gateway to expose backend endpoints.     

### Database:         
- Use AWS RDS for production-ready PostgreSQL hosting. 

# Usage
- Visit the deployed application in your browser.          
- Add, update, delete, and search inventory items using the Material UI Data Grid interface. 

# Contributors

- Mike Henke
- Benjamin Amoussou
- Katkoe Teko
- Patrick Nikiema
- Uladzimir Lahvinovich


### Additional Resources

- [AWS commands](https://github.com/ed-roh/inventory-management/blob/master/server/aws-ec2-instructions.md)

