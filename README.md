# 🏫 IS216 Web Application Development II - OnlyNotes
---

## Business Problem

The community problem our project aims to address is that we realise the process of purchasing notes in SMU to be a cumbersome process. Currently, a solution that exists is the AskSMU channel in Telegram, in which students can liaise with sellers through the Education Resources topic in the channel. However, this would mean offline communication, handling of payments, and sending of files. Such way of notes distribution and purchase is cumbersome. 

Further research on competitors shows that Studocu and CourseHero aims to solve similar issues. However, these notes on AskSMU do not have these notes being listed on the platforms. Upon further research, we realise the lack of incentivisation on the current platforms being a missing gap as to why the notes are not being published. Thus, we aim to build a marketplace that allows SMU students to purchase and sell notes for the community.

---

## Web Solution Overview

### 🎯 Intended Users
- SMU Students who are in need of notes for their modules
- SMU Studens who would want to sell their notes and earn some quick cash.

### 💡 What Users Can Do & Benefits

| Feature | Description | User Benefit |
|:--|:--|:--|
| Register & Login | Secure authentication system | Personalized experience and data security |
| Product Listing | View all notes within the web application | Users can view these notes and make a selection based on their wants. |
| Note Recommendation System | Find notes based on modules you have taken and time of the semester | Allows students to have quick access of the modules they are taking without having to search |
| Semantic Search | Allows for search based on note content and embeddings generated rather than normal text search | Quick search for notes users would need. |
| Node based knowledge graph  | Users can view information about their notes in the form of a graph, connecting different concepts and the relation between them as edges | Users can understand the meaning of the notes in a visual manner without much viewing before purchasing |
| Forum | Buyers can leave comments and question on certain parts of the notes they own for sellers. Sellers can answer these questions. | Creates a form of communication between buyers and sellers after purchasing a certain note for clarification. |
| Seller Dashboard | Sellers can view key metrics on the notes they sold and their performance.  | Sellers can analyse and know how to improve on their sales. They would know which notes to sell, and at certain price points. |
| Compose Notes | Rather than uploading notes, sellers can write their own notes within the application and post them as articles for students to view.  | Sellers can create notes on the go, rather than uploading a certain note in their computer. |
| Payment for notes | Students can purchase their notes on the application.  | Allows student to link their card and pay via stripe API. |
---

## Tech Stack

### 🧱 Tech Stack Overview

#### Frontend
| Logo | Technology | Purpose / Usage |
|:--:|:--|:--|
| <img src="https://raw.githubusercontent.com/github/explore/main/topics/react/react.png" width="40"> | **React** | Frontend framework for building dynamic user interfaces |
| <img src="https://raw.githubusercontent.com/github/explore/main/topics/tailwind/tailwind.png" width="40"> | **TailwindCSS** | Utility-first CSS framework for styling and responsive layouts |
| <img src="https://raw.githubusercontent.com/shadcn/ui/main/apps/www/public/og.jpg" width="40"> | **Shadcn/UI** | Pre-built accessible UI components styled with TailwindCSS |
| <img src="https://vitejs.dev/logo.svg" width="40"> | **Vite** | Lightning-fast development server and build tool |

#### Backend
| Logo | Technology | Purpose / Usage |
|:--:|:--|:--|
| <img src="https://raw.githubusercontent.com/github/explore/main/topics/nodejs/nodejs.png" width="40"> | **Node.js** | JavaScript runtime for backend execution |
| <img src="https://raw.githubusercontent.com/github/explore/main/topics/typescript/typescript.png" width="40"> | **TypeScript** | Strongly-typed superset of JavaScript for maintainable backend code |
| <img src="https://raw.githubusercontent.com/github/explore/main/topics/express/express.png" width="40"> | **Express.js** | Web framework for building RESTful APIs |
| <img src="https://raw.githubusercontent.com/github/explore/main/topics/docker/docker.png" width="40"> | **Docker** | Containerization for development process |

### Deployment
| Logo | Technology | Purpose / Usage |
|:--:|:--|:--|
| <img src="https://repository-images.githubusercontent.com/100966547/fc3c3680-355c-11eb-9554-8df45a88295b" width="40"> | **AWS Cognito** | User authentication and authorization service |
| <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQUlDqQ4KhvbzAUcyYoAvroy03MDJontu8baA&s" width="40"> | **AWS ECS** | Container orchestration for backend microservices |
| <img src="https://avatars.githubusercontent.com/u/41077760?s=200&v=4" width="40"> | **AWS Amplify** | Hosting and CI/CD for the frontend React app |

#### Data
| Logo | Technology | Purpose / Usage |
|:--:|:--|:--|
| <img src="https://raw.githubusercontent.com/github/explore/main/topics/mongodb/mongodb.png" width="40"> | **MongoDB** | NoSQL database for document-oriented data storage |
| <img src="https://raw.githubusercontent.com/github/explore/main/topics/supabase/supabase.png" width="40"> | **Supabase** | Postgres-based backend-as-a-service for structured data |
| <img src="https://user-images.githubusercontent.com/15157491/75435753-6929fc80-594b-11ea-9e19-f78223916862.png" width="40"> | **AWS S3** | Object storage for images, files, and note uploads |
| <img src="https://e7.pngegg.com/pngimages/890/101/png-clipart-rabbitmq-advanced-message-queuing-protocol-message-queue-computer-network-others-miscellaneous-computer-network-thumbnail.png" width="40"> | **RabbitMQ** | Message broker for asynchronous communication between services |

---

## Use Case & User Journey

Provide screenshots and captions showing how users interact with your app.
For the testing of the web application, we have tested from viewport of 375 px (Iphone 6/7/8) to Bootstrap XL, based on the projet requirements.

#### Introduction
1. **Landing Page**  
   <img src="screenshots/landing.png" width="600">  
   - Displays the homepage introducing OnlyNotes with options to browse or sell notes, followed by sections highlighting platform benefits, step-by-step guides for buyers and sellers, curated study roadmaps for guidance, and recommended notes.

2. **Register & Login**  
   <img src="screenshots/register.png" width="600">  
   <img src="screenshots/login.png" width="600">  
   - Users can register for an account and login.

3. **Note Recommendation System**  
   <img src="screenshots/noterecommendation.png" width="600">  
   - Users can find notes based on modules they have taken and time of the semester


#### Search
1. **Product Listing**  
   <img src="screenshots/productlisting.png" width="600">  
   - Users are able to view notes put up by other users.

2. **Roadmap**  
   <img src="screenshots/roadmap.png" width="600">  
   - Users can also reference a roadmap based on their degree to search for desired notes.

3. **Semantic Search**  
   <img src="screenshots/semanticsearch.png" width="600">  
   - User can search based on note content and embeddings generated rather than normal text search.

4. **Node based knowledge graph**  
   <img src="screenshots/nodeknowledgegraph.png" width="600">  
   - Users can summarize and view notes in a graph form showing connected concepts and relationships. 


### Create
1. **Compose Notes**  
   <img src="screenshots/compose.png" width="600">  
   - Users can choose to create their own notes on the platform.

2. **Upload Notes**  
   <img src="screenshots/uploadNotes_1.jpg" width="600">  
   <img src="screenshots/uploadNotes_2.jpg" width="600">  
   <img src="screenshots/uploadNotes_3.jpg" width="600">  
   <img src="screenshots/uploadNotes_4.jpg" width="600">  
   <img src="screenshots/successUpload.png" width="600">  
   - Users can choose to upload via 4 step process.


#### Purchase
1. **Stripe payment**  
   <img src="screenshots/stripePayment.jpg" width="600">  
   - Users are able to purchase notes.
2. **Confirmation Pages**  
   <img src="screenshots/paymentSuccessful.jpg" width="600">  
   - Successful status.
   <img src="screenshots/paymentFailed.jpg" width="600">  
   - Unsuccessful status.


#### Discuss
1. **Forum**  
   <img src="screenshots/forum.png" width="600">  
   - Users can discuss in a forum regarding their purchased notes, specific text quotes can be highlighted for reference.


#### Dashboard
1. **Seller Dashboard**  
   <img src="screenshots/dashboard1.png" width="600">  
   <img src="screenshots/dashboard2.png" width="600">  
   - Users can view key metrics regarding the performance of their notes.

---
