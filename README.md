# summerintership2024_22IT116
<h2>4th Sem Summer Internship</h2>

## 🚀 Introduction
This repository documents my one-month summer internship experience at Izonnet Web Solution Pvt. Ltd. During this internship, I underwent two weeks of intensive training followed by two weeks of hands-on project work, focusing on the MERN (MongoDB, Express.js, React, Node.js) stack.

### *15th May 2024*
# Start of Internship
## 1️⃣ week 1

## 📝 Day-by-Day Progress

### Day 1: Creating AWS Free Tier Account
- Introduction to the MEAN stack, its components, and setup.
- Installing and setting up MongoDB, and understanding its basics.
- Creating a simple MongoDB database and  performing CRUD operations.


### Day 2: creating instance with apache server to deploy web page
➠Introduction to Node.js and its environment 

➠ Learning the basics of Express.js and setting up a server 

➠ Installed an Apache Web Server on the Linux Instance (Task 7):
- Once connected, I installed Apache, a widely-used open-source web server software. Apache is crucial for serving web pages to users. The installation involved updating the package repositories and using package management commands to install Apache on the Linux-based EC2 instance.

➠ Commands : 
- sudo su-to elevate your credentials to root
- yum install -y httpd- to install apache web server(Linux server)
- cd /var/www/html- to create a HTML file into directory

➠Deployed a Personal page.html on Apache (Task 8):
- With Apache running, I deployed a simple HTML page (Personalpage.html). This involved placing the HTML file in Apache’s root directory and 
  configuring the server to serve this page. Deploying the HTML page allowed me to create a personal webpage accessible over the internet via 
  the EC2 instance's public IP address.

### Day 3: Building the Portfolio

➠ Setting Up the Project Structure:
- Created a project directory on the EC2 instance for the portfolio website. This included folders for HTML, CSS, JavaScript, and assets like images and fonts.
- Initialized the project with a basic index.html file to serve as the homepage.

➠ Creating the HTML Structure:
- Developed the initial structure of the portfolio using HTML5. This involved creating sections for the header, about me, projects, and contact information.
- Ensured the HTML code was semantic and well-organized to improve readability and SEO.

➠ Integrating Bootstrap:
- Incorporated Bootstrap, a popular CSS framework, to make the portfolio responsive and visually appealing.
Used Bootstrap components like navigation bars, cards, and buttons to enhance the design and functionality of the website.

### Day 4: Enhancing with JavaScript, SASS, and CSS

➠Adding Interactivity with JavaScript:
- Implemented JavaScript to add interactive features to the portfolio, such as form validation for the contact section and dynamic content loading for the projects section.
Utilized event listeners and DOM manipulation to create a more engaging user experience.

➠ Styling with SASS and CSS:
- Used SASS (Syntactically Awesome Style Sheets) to write more maintainable and modular CSS code. SASS variables, nesting, and mixins helped streamline the styling process.
- Compiled SASS files into CSS and applied custom styles to enhance the visual aesthetics of the portfolio. This included customizing Bootstrap themes and adding unique design elements.

➠ Finalizing the Deployment:
- Ensured all the files were correctly linked and the website was functioning as intended.
- Tested the portfolio on different browsers and devices to ensure compatibility and responsiveness.

➠Technologies Explored
- HTML5: Structured the content and elements of the portfolio.
- Bootstrap: Provided a responsive and modern design framework.
- JavaScript: Added interactivity and dynamic functionality to the website.
- SASS: Enhanced the CSS with advanced features for better maintainability and efficiency.
- CSS: Styled the website to improve visual appeal and user experience.

### Day 5: Configuration and final Touchup
- Configured the Security Group for the Apache server on the EC2 instance to accept incoming connections on port 80. This involved adding an inbound rule in the Security Group settings to allow HTTP traffic, ensuring that the web server is accessible from the internet.(Task 9)

- Verified the configuration by accessing the personal webpage hosted on the EC2 instance. Used the public IP address of the instance in a web browser to confirm that the Apache server is serving the webpage correctly. This demonstrated successful setup and configuration of the web server.(Task 10)

- Here is the finalised link : http://52.63.0.141/personalpage.html

## Notes:
➠We were given this repo which contains basic documentation of AWS services which can be helpful to everybody --
https://github.com/hamidgholami/accp-cheatsheet

## 2️⃣ week 2

### *4th June 2024*
- *Online Session*: Learning about storage and S3 with its related services ,also swictching from EC2 to S3
- In the start of meeting we were asked rapid questions regarding week 1 task.
  ![AWS Cloudfront](https://media.licdn.com/dms/image/C4E12AQEYszsOFAPr5w/article-cover_image-shrink_423_752/0/1604073753428?e=1723680000&v=beta&t=jL2yIMG8R1YzgOTl7VSfr4YN6m50WtYwZTvAFLipRRE)


### *Here is the Outine of Week-2:*
1. Create a Bucket
2. Make it private
3. Upload files
4. Encrypt the files
5. Create a Distribution 
6. Integrate it with S3
7. Create a new KMS Key
8. Change the Default Key for your bucket to this new key
9. Find out these events and logs for them in Cloudtrail
10. Shutdown the EC2 instance we created in first week

## 📝 Day-by-Day Progress

### Day 1: Creating and Configuring an S3 Bucket
➠ Created a new S3 bucket:
- I started by creating a new Amazon S3 bucket. Amazon S3 is a scalable object storage service that allows for the storage and retrieval of any amount of data at any time.
 
➠ Set the bucket's permissions to private:
- Ensured the bucket's security by setting its permissions to private, making sure that only authorized users have access to the stored data.
  
➠ Uploaded files to the bucket:
- Uploaded various files to the S3 bucket to test storage and retrieval capabilities. This provided hands-on experience with S3's upload functionalities and permissions settings.

### Day 2: Securing and Distributing Content
➠ *Enabled encryption for the uploaded files*:
  - To enhance data security, I enabled server-side encryption for the files uploaded to the S3 bucket. This ensures that data is encrypted at rest, protecting it from unauthorized access.
    
➠ *Created a CloudFront distribution and integrated it with the S3 bucket*:
  - Created an Amazon CloudFront distribution to deliver content stored in the S3 bucket with low latency and high transfer speeds. This involved setting up the distribution and linking it to the S3 bucket, demonstrating how CloudFront can improve content delivery performance.

- CDN(Content Delivery Network) --

<img src="https://d1.awsstatic.com/products/cloudfront/product-page-diagram_CloudFront_HIW.475cd71e52ebbb9acbe55fd1b242c75ebb619a2e.png" width="550" height="300"/>

### Day 3: Advanced Security and Monitoring

➠ Created a new KMS key:
- Created a new AWS Key Management Service (KMS) key to manage encryption keys. KMS provides centralized control over encryption keys, enhancing data security.
   
➠ Changed the default encryption key for the S3 bucket to the new KMS key:
- Configured the S3 bucket to use the newly created KMS key for default encryption. This ensures that all future objects uploaded to the bucket are encrypted using the KMS key, providing an additional layer of security.
   
➠ Used CloudTrail to track events and logs related to the S3 bucket and other activities:
- Utilized AWS CloudTrail to monitor and log activities related to the S3 bucket. CloudTrail provides visibility into API calls and user actions, aiding in compliance and security analysis.
   
➠ Shut down the EC2 instance created in Week 1:
- As part of resource management and cost control, I shut down the EC2 instance that was set up during the first week. This practice helps avoid unnecessary charges and optimizes resource usage.

### In Day 4-5 i was supposed to explore and learn new services in brief by my own

### Day 4: Discovering AWS Athena's Capabilities

➠ Explored the versatility of SQL queries in AWS Athena
  - Investigated the range of SQL queries possible in AWS Athena, understanding how it interacts with data stored in S3 and the types of analysis that can be performed.
    
➠ Examined data partitioning strategies*:
  - Studied various data partitioning strategies and their impact on query performance in Athena, gaining insights into how partitioning contributes to cost savings.
    
➠ Learned about AWS Glue Data Catalog integration
  - Explored how AWS Glue Data Catalog serves as a central metadata repository and how it integrates with Athena to make S3 data easily searchable and queryable.

### Day 5: Exploring Data Integration and Orchestration

➠ Investigated AWS Glue's ETL capabilities
  - Researched AWS Glue's ETL features, understanding how it automates the extraction, transformation, and loading of data for analytics.
    
➠ Familiarized with AWS Step Functions' orchestration
  - Learned about AWS Step Functions and its ability to coordinate multiple AWS services into serverless workflows, grasping the basics of service orchestration.
    
➠ Reviewed error handling in Step Functions workflows*:
  - Reviewed best practices for implementing error handling in Step Functions workflows, appreciating the importance of resilience in service orchestration.

## 3️⃣ week 3

### 12th June 2024
- Online Session: Introduction to AWS DynamoDB, API Gateway, and Lambda Functions
- This week focused on building a serverless backend using AWS services like DynamoDB, API Gateway, and Lambda Functions. We worked on a project to create CRUD APIs for managing items in a DynamoDB table.

  <img src="https://media.licdn.com/dms/image/D5612AQFMBfd4HnZ0Iw/article-cover_image-shrink_720_1280/0/1699630089018?e=1724284800&v=beta&t=eG1tqVAl1EvKAu9J4LmAqAmFE5uxPQReQJEz88P8xiA" width="550" height="300"/>


### Here is the Outline of Week-3:
1. Create a table in DynamoDB
2. Write a Lambda Function as a Backend
3. Configure API Endpoints on API Gateway
4. Get /items
5. Put /items
6. Get /items/{id}
7. Delete /items/{id}
8. Configure API Endpoints with Lambda Code
9. Test Out APIs through Curl and Browser

## 📝 Day-by-Day Progress

### Day 1: Creating a Table in DynamoDB

➠ Create a table in DynamoDB
- Created a new table in Amazon DynamoDB. DynamoDB is a fast and flexible NoSQL database service for all applications that need consistent, single-digit millisecond latency at any scale. I configured the table with a primary key and other necessary attributes to store item data efficiently.

  ### Day 2: Writing Lambda Functions
  
➠ Write a Lambda Function as a Backend
- Developed a Lambda function to serve as the backend logic for our CRUD operations. AWS Lambda allows you to run code without provisioning or managing servers. The function was written in Python and included logic to interact with DynamoDB for various operations like retrieving, inserting, updating, and deleting items.

### Day 3: Configuring API Endpoints

➠ Configure API Endpoints on API Gateway
- Set up API Gateway to expose our Lambda functions as RESTful API endpoints. Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. Configured the endpoints for the various CRUD operations.

### Day 4: Implementing CRUD Operations

➠ *Get /items
- Configured the GET /items endpoint to retrieve all items from the DynamoDB table. This endpoint interacts with the Lambda function to fetch and return the list of items.

➠ Put /items
- Set up the PUT /items endpoint to add new items to the DynamoDB table. The Lambda function processes the incoming request and inserts the new item into the table.

➠ Get /items/{id}
- Implemented the GET /items/{id} endpoint to retrieve a specific item by its ID. The Lambda function uses the ID parameter to query DynamoDB and return the requested item.

➠ Delete /items/{id}
- Configured the DELETE /items/{id} endpoint to remove an item from the DynamoDB table based on its ID. The Lambda function handles the deletion process and ensures the item is removed.

➠ Configure API Endpoints with Lambda Code
- Linked the API Gateway endpoints with the corresponding Lambda functions. This integration allows API Gateway to invoke the correct Lambda function for each API request, ensuring the backend logic is executed properly.

➠ Test Out APIs through Curl and Browser
- Tested the configured APIs using curl commands and a web browser to ensure they work as expected. Verified that the CRUD operations (Create, Read, Update, Delete) perform correctly and that the APIs return the appropriate responses for different scenarios.


## 4️⃣ week 4

### *21st June 2024*
- *Online Session*: Introduction to AWS Bedrock, S3, and Knowledge Base Integration
- This week focused on building a knowledge base using AWS Bedrock, creating a vector store for efficient data retrieval, and interacting with the knowledge base using an agent.

  <img src="https://community.aws/_next/image?url=https%3A%2F%2Fassets.community.aws%2Fa%2F2Z6yg51zfyrwr7WzyFJ4zNsUukb.png%3FimgSize%3D2772x1102&w=3840&q=75" width="550" height="300"/>

### *Here is the Outline of Week-4:*
1. Create a Bucket
2. Upload my Resume
3. Create Knowledge Base in BedRock
4. Link S3 Bucket Object (Resume) with this Knowledge Base
5. Create Vector Store using Embeddings and Data Source
6. Test Knowledge Base using Generate Responses
7. Test Knowledge Base without using Generate Responses
8. Create an Agent
9. Connect it with Knowledge Base
10. Interact with your Resume

## 📝 Day-by-Day Progress

### Day 1: Setting Up the S3 Bucket and Uploading Resume

➠ Create a Bucket
- Created a new S3 bucket for storing objects. Amazon S3 is a scalable object storage service that allows for the storage and retrieval of any amount of data at any time.

➠ Upload my Resume
- Uploaded my resume to the S3 bucket. This step is crucial for linking the resume to the knowledge base in Bedrock.

### Day 2: Creating and Linking Knowledge Base in Bedrock

➠ Create Knowledge Base in BedRock
- Created a knowledge base in AWS Bedrock. Bedrock is used for building intelligent applications with comprehensive knowledge management and natural language understanding capabilities.

➠ Link S3 Bucket Object (Resume) with this Knowledge Base
- Linked the uploaded resume from the S3 bucket to the knowledge base. This allows Bedrock to use the resume as a data source for generating responses.

### Day 3: Building and Testing the Vector Store

➠ Create Vector Store using Embeddings and Data Source
- Created a vector store using embeddings to enable efficient data retrieval. This involved transforming the resume data into vector embeddings that Bedrock can use for quick search and retrieval.

➠est Knowledge Base using Generate Responses
- Tested the knowledge base by generating responses from the linked resume data. This helped verify that the knowledge base correctly understands and retrieves information from the resume.

➠ Test Knowledge Base without using Generate Responses
- Conducted tests on the knowledge base without using the generate response feature to ensure it can handle direct queries and return accurate information.

### Day 4: Creating and Connecting an Agent

➠Create an Agent
- Created an agent in AWS Bedrock. Agents in Bedrock are responsible for interacting with users and providing responses based on the knowledge base.

➠Connect it with Knowledge Base
- Linked the created agent with the knowledge base to enable it to access and retrieve information from the resume stored in S3.

### Day 5: Interacting with the Resume

➠Interact with your Resume
- Interacted with the resume through the agent. This involved querying the agent to retrieve specific information from the resume, ensuring the setup was functional and effective.

## Problems faced after few Days of competion of Internship

- After completion of Internship on 30 June I came across the mails that my billing charges are getting than we are expecting.
- Then I contact Amit Aurora sir and he helped me and we come to know that my bedrock,KMS,Agent Services are still on.
- then we conatact to AWS support and wrote them that we are student and we were exploring the servies and went dee,it was not intentionally
- then we go reply for few days and i reply them back everyday like they were mailing me to xyz servies are still on and terminate them
- iused to terminate them accordingly and sending them attachment for proof and on 15 july the billing things was sorted out
- all thnaks to AWS and Amit sir for Guiding me


## 🤝 Connect with Me

- LinkedIn: [[https://www.linkedin.com](https://www.linkedin.com/in/viken-hadavani-27b6412b3?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3Bc%2BtFz8i0SqaVmf395szcFw%3D%3D)]

- Email: [vikenhadavani@gmail.com]


Thank you for visiting my project! Feel free to reach out if you have any questions or feedback. ✨
