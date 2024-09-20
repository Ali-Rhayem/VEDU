<img src="./readme/title1.svg"/>

<br><br>

<!-- project philosophy -->
<img src="./readme/title2.svg"/>

> A comprehensive virtual classroom platform designed to facilitate seamless online teaching and learning, empowering both instructors and students through advanced technology.
>
> VEDU aims to revolutionize the learning experience by integrating advanced AI technologies, creating an engaging, interactive, and efficient environment. Our philosophy focuses on accessibility, personalization, and collaboration, enhancing both teaching and learning through technology.

### User Stories

#### Instructor

- As an instructor, I want to use Google Meet with live video, audio, and screen sharing, so I can conduct interactive classes and present my materials effectively.
- As an instructor, I want to engage with students through live chat within each class, so I can answer questions and facilitate discussions during the session.
- As an instructor, I want to use a collaborative compiler where only I can edit unless I give permission to students, so I can control who contributes to coding tasks during live sessions.
- As an instructor, I want to use a Chrome extension that summarizes chat discussions, so I can review key points and follow up on class interactions efficiently.

#### Student

- As a student, I want to participate in class via Google Meet with video, audio, and screen sharing, so I can fully engage in live sessions and discussions.

- As a student, I want to use live chat during the class to ask questions or share my thoughts without interrupting the flow of the session.

- As a student, I want to work with a collaborative compiler, but only edit code when the instructor gives permission, so I can contribute to coding tasks when appropriate.

- As a student, I want to interact with an AI assistant during class to ask questions and receive instant responses, so I can get personalized help when I need it.

- As a student , I want to use a Chrome extension that summarizes chats , so I can follow up on class interactions efficiently.

<br><br>

<!-- Tech stack -->
<img src="./readme/title3.svg"/>
<br><br>

### VEDU is built using the following technologies:

- The frontend was built using **[React](https://react.dev)**. React is a front-end JavaScript library based on components, it is like creating building blocks and then stacking them on each other to build a website.
- The backend was built using **[Laravel](https://laravel.com/docs/11.x/releases)** for handling backend logic and API operations, and **[Node.js](https://nodejs.org/en)** with **[Socket.IO](https://socket.io)** for real-time features like live sockets, the collaborative compiler, and chat functionality.
- For the database, **[MySQL](https://www.mysql.com)** was chosen for its reliability, performance, and scalability. Its support for ACID transactions and optimized indexing makes it ideal for handling real-time functionalities efficiently.
- For the frontend routing, **[React Router v6.21](https://reactrouter.com/en/6.21.3/start/overview)** was used, which made routing on the frontend easier and working with data better with its data API.

- For real-time collaboration in compiler, and real time messaging ,the app uses **[Socket.IO](https://socket.io)**, a library that enables low-latency, bidirectional, and event-based communication between the client and server, allowing multiple users to chat and edit code collaboratively in real time.

<br><br>

<!-- UI UX -->
<img src="./readme/title4.svg"/>
<br><br>

> We designed VEDU using wireframes and mockups, iterating on the design until we reached the ideal layout for easy navigation and a seamless user experience.

- Project Figma design [figma](https://www.figma.com/file/LsuOx5Wnh5YTGSEtrgvz4l/Purrfect-Pals?type=design&node-id=257%3A79&mode=design&t=adzbABt5hbb91ucZ-1)

### Mockups

| Register screen                             | Chatting Screen                           | Compiler Screen                          |
| --------------------------------------- | ------------------------------------- | ------------------------------------- |
| ![Register](./readme/demo/Register.png) | ![Chatting_Page](./readme/demo/Chatting_Page.png) | ![Compiler](./readme/demo/Compiler.png) |

<br><br>

<!-- Database Design -->
<img src="./readme/title5.svg"/>

### Architecting Data Excellence: Innovative Database Design Strategies:

<img src="./readme/demo/Database.png">

<br><br>

<!-- Implementation -->
<img src="./readme/title6.svg"/>

### User Screens (Mobile)

| Login screen                                    | Register screen                               |
| ----------------------------------------------- | --------------------------------------------- |
| ![Login](./readme/demo/Login.png)               | ![Register](./readme/demo/Register.png)       | 
| Home Page                                       | Class Page                                    |
| ![Home](./readme/demo/Home.png)                 | ![Class](./readme/demo/Class.png)             | 
| Landing Page                                    | Assignments Page                              |
| ![Landing](./readme/demo/Landing.gif)           | ![Assignments](./readme/demo/Assignments.png) |
| Submissions Page                                | Chats Page                                    |
| ![Submissions](./readme/demo/Submissions.png)   | ![Chats](./readme/demo/Chats.png)             |
| Chat Page                                       | Class People Page                             |
| ![Chat](./readme/demo/Chatting_Page.png)        | ![Classpeople](./readme/demo/Class_People.png)|
| Meeting Setup Page                              | Video Call Page                               |
| ![Setup Page](./readme/demo/Meeting_Setup_Page.png)| ![Videocall](./readme/demo/Video_call.gif) |
| compiler                                        | Real Time coding                              |
| ![Compiler](./readme/demo/Compiler.png)         | ![Videocall](./readme/demo/Live_coding.gif)   |

### Admin Screens (Web)

| Login screen                            | Register screen                       | Landing screen                        |
| --------------------------------------- | ------------------------------------- | ------------------------------------- |
| ![Landing](./readme/demo/1440x1024.png) | ![fsdaf](./readme/demo/1440x1024.png) | ![fsdaf](./readme/demo/1440x1024.png) |
| Home screen                             | Menu Screen                           | Order Screen                          |
| ![Landing](./readme/demo/1440x1024.png) | ![fsdaf](./readme/demo/1440x1024.png) | ![fsdaf](./readme/demo/1440x1024.png) |

<br><br>

<!-- Prompt Engineering -->
<img src="./readme/title7.svg"/>

### Mastering AI Interaction: Unveiling the Power of Prompt Engineering:

- This project uses advanced prompt engineering techniques to optimize the interaction with natural language processing models. By skillfully crafting input instructions, we tailor the behavior of the models to achieve precise and efficient language understanding and generation for various tasks and preferences.

<br><br>

<!-- AWS Deployment -->
<img src="./readme/title8.svg"/>

### Efficient AI Deployment: Unleashing the Potential with AWS Integration:

- This project leverages AWS deployment strategies to seamlessly integrate and deploy natural language processing models. With a focus on scalability, reliability, and performance, we ensure that AI applications powered by these models deliver robust and responsive solutions for diverse use cases.

<br><br>

<!-- Unit Testing -->
<img src="./readme/title9.svg"/>

### Precision in Development: Harnessing the Power of Unit Testing:

- This project employs rigorous unit testing methodologies to ensure the reliability and accuracy of code components. By systematically evaluating individual units of the software, we guarantee a robust foundation, identifying and addressing potential issues early in the development process.

<br><br>

<!-- How to run -->
<img src="./readme/title10.svg"/>

> To set up Coffee Express locally, follow these steps:

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.

- npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._

1. Get a free API Key at [example](https://example.com)
2. Clone the repo
   git clone [github](https://github.com/your_username_/Project-Name.git)
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = "ENTER YOUR API";
   ```

Now, you should be able to run Coffee Express locally and explore its features.
