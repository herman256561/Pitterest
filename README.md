**Welcome to Pitterest!! 🥳 🥳**

## Introduction
---
### Project Overview 🌆
**"Pitterest"** is an interactive web platform inspired by the layout of Pinterest and the functionality of Reddit, customized for the unique context of the greater Pittsburgh area. It is designed to showcase people's unique experiences, attractions, and anything else related to Pittsburgh. Pittsburghers can share their daily encounters with novel and interesting things, as well as their discoveries and experiences, which will be displayed on a communal homepage, revealing the diverse tapestry of life in Pittsburgh. This platform aims to foster a community of curious individuals who delight in exploring unique moments, places, and items they encounter in their daily lives. Additionally, it encourages exploration of activities, events, architecture, and the distinct vibes of different neighborhoods.

### About our team 🙋‍♂️👩‍💼🧑‍💻🦸‍♂️
**We are Pitt Crafters!**
Our team consists of four master’s students in Information Science at the University of Pittsburgh: Pei-Chieh Chen (pec111), Si-Lian Wu (siw92), Che-Hsuan Cho (chc526), and Chenglue Huang (chh313). United by our appreciation for Pittsburgh's fun, playful, and artistic atmosphere, we aim to enrich community interaction by making local sharing and recommendations more accessible and engaging.

### Project Demo
[Click Here To Watch Project Demo](https://youtu.be/s7crGKuJhOQ)

---
## Objective
---
Describe with more specific details what your objectives and goals are for the project. What problems did you want to solve or what did you want to learn in developing this application? What features, beyond the ones listed in the assignment requirements, did you implement?
### The Problem 🔍
While we love living in this city, renowned for its vibrant, fun, and artistic ambiance, we have observed a gap in the sharing of recommendations for interesting experiences or recommended activities/places in daily life among community members. Local insights, recommendations, and life experience sharing are often dispersed and not readily accessible to the people in this community who are seeking to explore something new in Pittsburgh. This lack of a centralized platform for sharing local experiences can make it difficult for individuals to uncover the city's hidden gems.
### The Solution 🎯
To address this, we are driven to create "Pitterest," a platform designed for the residents of the greater Pittsburgh area that categorizes and highlights different aspects of life in Pittsburgh

### Features
#### Categorized Sharing
Users can post their experiences and recommendations under specific categories, enhancing accessibility and relevance.
:::success
* Landmarks and Attractions: 
Highlight popular landmarks and attractions in Pittsburgh such as the Andy Warhol Museum, Phipps Conservatory, the Pittsburgh Zoo, or the Duquesne Incline.
* Food and Dining: 
Showcase local cuisine and dining spots unique to Pittsburgh, including famous dishes like Primanti Brothers sandwiches, pierogies, and local breweries or coffee shops.
* Outdoor Activities: 
Pin images and information about outdoor activities in Pittsburgh, such as hiking trails in Frick Park, kayaking on the Three Rivers, or biking along the Great Allegheny Passage.
* Events and Festivals: 
Feature upcoming events and festivals in Pittsburgh, like the Three Rivers Arts Festival, the Pittsburgh Marathon, or Steelers and Pirates games.
* Architecture and History: 
Share pins highlighting the unique architecture and historical sites in Pittsburgh, such as the Cathedral of Learning, the Carrie Furnaces, or the Heinz History Center.
* Neighborhoods: 
Create sections dedicated to different neighborhoods in Pittsburgh, such as the Strip District, Lawrenceville, Shadyside, or Squirrel Hill, showcasing their distinct vibes and attractions.
:::

#### Make Posting Process Easier
The website simplifies the posting process, guiding users through adding detailed information such as location information, categories, hashtags, and relevant links. This ensures that content is not only engaging but also informative and easy to navigate.

#### Dashboard for Content Management
Users can manage their content through a comprehensive dashboard, where they can edit or delete posts individually or in batches. This feature supports active community engagement and content curation, making it easy for users to keep their contributions relevant and up-to-date.

#### Enhanced User Experience
Pitterest is designed to simplify the workflow for sharing ideas, experiences, and recommendations. By focusing on user interface and interaction, the platform ensures a smooth and enjoyable experience for all users, encouraging more frequent and meaningful interactions within the community.

### Functionalities
#### Display Post
* **Description:** All user posts are displayed on a communal board, allowing for easy access and interaction.

#### Sign Up & Log In
* **Description:** Users have the ability to sign up for an account and log in to access personalized features. Express.js session is used to check user's session and keep the login status.

#### Manage Post
* **Description:** Users can create, edit, and delete their own posts through a user-friendly dashboard.

#### Admin Role
* **Description:** Admin users have the authority to manage all posts, including editing and deleting any user post.



## Team member’s contributions 🙋‍♂️👩‍💼🧑‍💻🦸‍♂️
---
* 🎨 **Design**: Pei-Chieh Chen
* 🖥️ **Front-end**: Pei-Chieh Chen, Che-Hsuan Cho, Si-Lian Wu
* 💻 **Back-end**: Che-Hsuan Cho, Si-Lian Wu, Chenglue Huang
* 🗄️ **Database Design**: Pei-Chieh Chen, Che-Hsuan Cho
* 🚀 **Agile Development - Scrum**: Si-Lian Wu
* 📋 **Documentation**: Pei-Chieh Chen
* 💁 **Presentation**: Pei-Chieh Chen, Si-Lian Wu

## Technical Architecture
---
Our project follows the Model-View-Controller (MVC) architectural pattern, which separates the application into three interconnected components. This separation allows for efficient code management and simplifies the development process. Here's how we've utilized this model:

### Model 
* ✅ [**MongoDB**](https://www.mongodb.com) | 
Chosen for its flexibility and performance with large volumes of data.
* ✅ [**Mongoose**](https://mongoosejs.com) | 
A MongoDB object modeling tool designed to work in an asynchronous environment.
#### **Used for** 
* User Collection: Handles user data including username, password, name, and related personal information.
* Post Collection: Handles all data related to posts including title, location, category, and post related information.

### View
* ✅ **HTML**
* ✅ **CSS** | 
Structures and styles the website.
* ✅ [**Bootstrap**](https://bootstrapdoc.com) | 
Ensures the website is responsive and aesthetically pleasing across various devices.

#### **Used for**
* Home View: Displays the homepage with various categories of posts.
* Profile View: Shows individual user profiles with editable fields and posted content.
* Personal Manage View: Provides a dashboard for users to manage their posts.
* Admin View: Provides a dashboard for admins to manage posts.

### Controller
* ✅ [**Node.js**](https://nodejs.org/en)
* ✅ [**Express.js**](https://expressjs.com) | 
These form the backbone of our server-side logic, handling routing and request management.
* ✅ [**Express Session**](https://www.npmjs.com/package/express-session) | 
Middleware for session management in Express applications. It stores session data on the server and helps manage user sessions with cookies.
* ✅ [**dotenv**](https://www.npmjs.com/package/dotenv) | 
A zero-dependency module that loads environment variables from a `.env` file into `process.env`, providing a safe way to store configuration details separate from code.
* ✅ [**Node Fetch**](https://www.npmjs.com/package/node-fetch) | 
A lightweight module that brings `window.fetch` to Node.js, it allows server-side code to perform HTTP requests in a way similar to frontend code.
* ✅ **Node.js Path Module** | 
For working with file and directory paths, making it easier to handle and transform file paths.

#### **Used for**
* Authentication Controller: Manages user login and registration.
* Post Controller: Handles CRUD operations for posts and interacts with the Post model for database transactions.


## Challenges
---
In developing the Pitterest, our team encountered several challenges that tested our problem-solving skills and understanding of new technologies:

### API Integration with MongoDB Atlas
Initially, we attempted to use direct API calls to MongoDB Atlas for implementing CRUD operations. This approach proved to be complex and less efficient due to the detailed setup and management of API requests needed for each data interaction. The learning curve for implementing secure and efficient API calls was steeper than anticipated, leading to a little bit of delays in development.

### Switch to Mongoose
To overcome the complexities of using MongoDB Atlas API directly, we transitioned to using Mongoose, a higher-level ORM that simplifies interactions with MongoDB. While this shift made data handling easier, it required a comprehensive review and overhaul of our existing codebase, which was time-consuming and introduced temporary setbacks in our development schedule.

### Collaborative Challenges with Glitch
Collaborating via Glitch posed its own set of challenges due to its lack of integrated CI/CD mechanisms. This limitation made it difficult to track and merge the contributions of team members efficiently, often leading to overlapping efforts or missed integrations of completed parts.

### Obstacles with Login Functionality
We encountered an unexpected constraint while developing the login functionality with Glitch, as it blocked POST requests, a standard method for handling form submissions. This required us to choose an alternative approach using the Fetch API, which is effective, but diverted us from conventional development practices and demanded additional effort to do troubleshooting and validation.

## Future Work
---
### Future Features
Given the constraint of time, we want to operate the basic functionality stable at the first phase. Looking forward, we plan to add more extended features that will enrich user experience and Practicality as below

#### 1. Image Display and Management 🖼️
Next feature that we plan to implement is allowing users to upload and display images in their posts. This will involve integrating more advanced file handling and storage solutions, for example, we may use cloud storage services like AWS to manage these media efficiently.

#### 2. Display experience or recommendation by Map view 🌎
Adding a map view feature that allows users to view experiences and recommendations by Google Map will not only enhance their immersive experience while exploring, but also help them locate the target near them or in a specific area of interest more easily and efficiently. To implement this, we will integrate a mapping API such as Google Maps. Additionally, we will need to ensure robust backend support for geospatial queries to retrieve data based on location efficiently.

#### 3. Interactive Post Features ❤️
We will also add functionality for users to comment on posts and express their likes which will encourage more interaction and engagement among users on our platform. By adding this, we will adjust our MongoDB schema to support storing and retrieving comments and likes associated with each post. 

#### 4. Statistic Data and Trending Topics 📊
After the Pitterest has been operational for some time and has accumulated considerable content on the platform, we will add features that display diagrams or infographics. These will highlight popular events, trending places, or restaurants that are frequently mentioned on the Pitterest, providing users with insights into what’s currently popular or gaining attention in the community of the great area of Pittsburgh. For this feature, we will need to implement analytics capabilities to process and analyze user data.

#### 5. Vendor Accounts 👨‍💼
In the long term, we plan to introduce vendor accounts. This will allow local businesses and cultural institutions to engage with the community by posting content related to their brands, services and products. This also will provide a potential revenue for the platform to operate substantially. Furthermore, in order to support the requirement of supporting more different user roles and permission, we will build a module for admin to manage different user roles, their permissions, and customized visibility.

## Conclusion
---
This course and project have really ramped up our tech skills. Diving into **Node.js** and **MongoDB**, we’ve moved from just knowing the theory to being able to actually build solid back-end systems. We’ve gotten way more comfortable with **HTML** and **CSS**, and now, **Bootstrap**'s tools for creating sleek designs are part of our toolkit.

We’ve also had the chance to play around with **Vue.js** and other **JavaScript frameworks**, which has been pretty eye-opening. It’s shown us how dynamic web apps can be and the value of using components to build them. Plus, getting the hang of **RESTful APIs** means we’re now set up to craft web services that talk to each other smoothly.

Wrapping up, we’re all set with a beefed-up set of skills in web tech that matter big time in the digital world. Looking ahead, we’ve got what it takes to jump into more complex web frameworks and keep up with tech’s fast pace.

## Admin Account
Account: admin <br> 
Password: pitterest_admin

## Resources
---
Those are the resources that we referred:

* [Expressjs](https://expressjs.com/en/5x/api.html)
* [Node.js v22.0.0 documentation](https://nodejs.org/docs/latest/api/)
* [MongoDB Documentation](https://www.mongodb.com/docs/)
* [Mongoose Documentation](https://mongoosejs.com/docs/guide.html)
* [w3schools](https://www.w3schools.com/)
* [w3schools-Bootstrap 4 Tutorial](https://www.w3schools.com/bootstrap4/default.asp)
* [w3schools-JavaScript Tutorial](https://www.w3schools.com/js/default.asp)
* [w3school-W3.CSS Tutorial](https://www.w3schools.com/w3css/default.asp)
* [Stack Overflow](https://stackoverflow.com)

---
Credit: This documentation is completed by Pei-Chieh Chen
