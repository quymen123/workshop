---
title : "Introduction"
date :  "2025-02-08" 
weight : 1 
chapter : false
pre : " <b> 1. </b> "
---


In today's evolving cloud computing industry, serverless architecture is attracting significant attention for its scalability, cost-effectiveness, and ease of maintenance. This project of mine will demonstrate how to build a simple single function (registration, login) with a Backend written in Nodejs, a Frontend written in Nextjs, using MongoDB database and deployed on AWS using EC2. This technology provides powerful tools to develop scalable and cost-effective web applications with minimal operating costs.

#### Why use Nodejs?
Node.js is a web performance application development platform that allows handling multiple connections simultaneously thanks to an asynchronous model. Using JavaScript for both client and server, Node.js has a rich ecosystem of libraries via npm, is easily extensible for application microservices, and is suitable for real-time applications. A large community and easy-to-learn syntax are also outstanding features of Node.js.

#### Why use Nextjs?
Next.js is a powerful framework for web application development, featuring SEO optimization capabilities through Server-Side Rendering (SSR) and Static Site Generation (SSG). It provides high performance thanks to code splitting and fast page loading. Next.js is also easy to use with a clear directory structure and automatic routing, helping programmers easily manage the application.
Additionally, this framework allows building APIs within the same project, creating seamlessness between front-end and back-end. With rich features like optimized images, CSS Modules, and TypeScript support, Next.js is suitable for modern projects. The large development community and rich documentation are also plus points that help users easily find support and information.

#### Why use MongoDB
MongoDB is a flexible NoSQL database that allows data to be stored in the form of documents, easily changing the structure without changing the schema. It supports data dispersion and horizontal scaling, helping to process large amounts of data with fast query speeds. MongoDB is also easy to integrate with many programming languages, offers powerful querying capabilities, and has a large support community, making it an ideal choice for modern applications.

#### Why use AWS EC2?
AWS EC2 (Elastic Compute Cloud) is a cloud computing service that allows flexible expansion, easy deployment and management of virtual servers in minutes. It provides high availability with multiple zones and regions, strong security, and easy integration with other AWS services. The on-demand payment model helps optimize costs, making it the ideal choice for modern application deployment.

#### The workshop includes 6 main sections
 1. [Introduction ](1-introduce/)
 2. [Preparation](2-preparation/)
    1. [Download Visual Studio Code](2-preparation/2.1-vscode/)
    2. [Create AWS EC2 and Connect instance](2-preparation/2.2-ec2/)
 3. [Deploy Backend on AWS EC2](3-deploybackend/)
 4. [Deploy Frontend on AWS EC2](4-deployfrontend/)
 5. [Test and review app](5-testing/)
 6. [Clean Resources](6-cleanup/)