<img src="./readme/title1.svg"/>

<br><br>

<!-- project philosophy -->
<img src="./readme/title2.svg"/>

> A comprehensive virtual classroom platform designed to facilitate seamless online teaching and learning, empowering both instructors and students through advanced technology.
>
> VEDU aims to revolutionize the learning experience by integrating advanced AI technologies, creating an engaging, interactive, and efficient environment. Our philosophy focuses on accessibility, personalization, and collaboration, enhancing both teaching and learning through technology.

### User Stories

#### Instructor

- As an instructor, I want to use Meeting with live video, audio, and screen sharing, so I can conduct interactive classes and present my materials effectively.
- As an instructor, I want to use a collaborative compiler where only I can edit unless I give permission to students, so I can control who contributes to coding tasks during live sessions.
- As an instructor, I want to use a Chrome extension that summarizes chat discussions, so I can review key points and follow up on class interactions efficiently.

#### Student

- As a student, I want to participate in class via Meeting with video, audio, and screen sharing, so I can fully engage in live sessions and discussions.
- As a student, I want to work with a collaborative compiler, but only edit code when the instructor gives permission, so I can contribute to coding tasks when appropriate.
- As a student, I want to interact with an AI assistant during class to ask questions and receive instant responses, so I can get personalized help when I need it.

#### Admin

- As an admin, I want to View website stats so that i can monitor platform performance.
- As an admin, I want to View users with details like profile picture, name, email, and role for user management.
- As an admin, I want to View classes with name, owner, student, and instructor counts for class management.

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

- The app uses **[Electron](https://www.electronjs.org)** to run the admin panel on different operating systems. It uses standard web technologies like HTML, CSS, and JavaScript.

<br><br>

<!-- UI UX -->
<img src="./readme/title4.svg"/>
<br><br>

> We designed VEDU using wireframes and mockups, iterating on the design until we reached the ideal layout for easy navigation and a seamless user experience.

- Project Figma design [figma](https://www.figma.com/design/5KURW960W275YsNUEoj3wZ/VEDU?node-id=0-1&t=q2RgT8Zwbfn374vt-1)

### Mockups

| Chatting Screen | Compiler Screen |
| --------------------------------------- | ------------------------------------------------- |
| ![Chatting_Page](./readme/demo/Chatting_Page.png) |![Compiler](./readme/demo/Compiler.png) |



<br><br>

<!-- Database Design -->
<img src="./readme/title5.svg"/>

### Architecting Data Excellence: Innovative Database Design Strategies:

<img src="./readme/demo/Database.png">

<br><br>

<!-- Implementation -->
<img src="./readme/title6.svg"/>

### User Pages (Web)

| Login Page                                           | Register Page                                  |
| ---------------------------------------------------- | ---------------------------------------------- |
| ![Login](./readme/demo/Login.png)                    | ![Register](./readme/demo/Register.png)        |
| Home Page                                            | Class Page                                     |
| ![Home](./readme/demo/Home.png)                      | ![Class](./readme/demo/Class.png)              |
| Landing Page                                         | Assignments Page                               |
| ![Landing](./readme/demo/Landing.gif)                | ![Assignments](./readme/demo/Assignments.png)  |
| Submissions Page                                     | Chats Page                                     |
| ![Submissions](./readme/demo/Submissions.png)        | ![Chats](./readme/demo/Chats.png)              |
| Chat Page                                            | Class People Page                              |
| ![Chat](./readme/demo/Chatting_Page.png)             | ![Classpeople](./readme/demo/Class_People.png) |
| Meeting Setup Page                                   | Video Call Page                                |
| ![Setup Page](./readme/demo/Meeting_Setup_Page.png)  | ![Videocall](./readme/demo/Video_call.gif)     |
| compiler                                             | Real Time coding                               |
| ![Compiler](./readme/demo/Compiler.png)              | ![Videocall](./readme/demo/Live_coding.gif)    |
| Live Meet Chat                                       | Meeting chat with ai                           |
| ![Meeting_Chat](./readme/demo/Live_meeting_chat.gif) | ![Ai Chat](./readme/demo/Chat_with_ai.gif)     |

### Admin Panel (Desktop)

| Dashboard screen                          | users                                    |
| ----------------------------------------- | ---------------------------------------- |
| ![Dashboard](./readme/demo/Dashboard.png) | ![users](./readme/demo/Manage_users.png) |
| Courses                                   |
| ![classes](./readme/demo/Courses.png)     |

<br><br>

<!-- Prompt Engineering -->
<img src="./readme/title7.svg"/>

### Mastering AI Interaction: Unveiling the Power of Prompt Engineering:

- Chat Summaries: The AI model is prompted to process long chat logs and extract the most important points, providing users with concise summaries. By structuring the prompts to guide the AI on what to focus on, the model can effectively summarize conversations while filtering out less relevant information.

- AI Chat in Meetings: During meetings, users can interact with an AI by asking questions or seeking assistance. Through prompt engineering, we tailor the instructions given to the AI, helping it generate appropriate, real-time responses that fit the context of the discussion. This enhances the overall meeting experience, making the AI a valuable assistant.

<br><br>

<!-- AWS Deployment -->
<img src="./readme/title8.svg"/>

### Efficient Deployment: Unleashing the Potential with AWS Integration

This project demonstrates the deployment of both **Node.js** and **Laravel** backends on AWS EC2, leveraging **Nginx** as a reverse proxy to handle traffic. By combining these technologies, the deployment is optimized for scalability, reliability, and performance, ensuring seamless integration and responsiveness.


### **Deployment Steps**

#### 1. **Set Up EC2 Instance**

- Launch an EC2 instance on AWS with Ubuntu.
- Configure security groups to allow:
  - **Port 22** (SSH) for access to the instance.
  - **Port 80** (HTTP) for web traffic.
  - **Port 3000** for Node.js server

#### 2. **SSH into the EC2 Instance**

```bash
ssh -i "key.pem" ubuntu@ec2-public-ip
```

#### 3. **Install Necessary Software**

- Update the package list and install Nginx, Node.js, and PHP for Laravel:

```bash
sudo apt update
sudo apt install nginx
sudo apt install nodejs npm
sudo apt install php-fpm php-mysql
```

#### 4. **Transfer Project Files to EC2**

- Use scp to transfer Node.js and Laravel project files from your local machine to the EC2 instance:

```bash
scp -i "your-key.pem" -r /path/to/laravel-backend ubuntu@ec2-public-ip:/var/www/laravel-backend
scp -i "your-key.pem" -r /path/to/node-backend ubuntu@ec2-public-ip:/var/www/node-backend
```

#### 5. **Install dependencies**

- Laravel: Install PHP dependencies using Composer.

```bash
cd /var/www/laravel-backend
composer install
```

- Node.js: Install Node.js dependencies.

```bash
cd /var/www/node-backend
npm install
```

#### 6. **Configure nginx**

- Edit the Nginx configuration file to act as a reverse proxy for both Node.js and Laravel:

```bash
sudo nano /etc/nginx/sites-available/default
```

- Add the following to route traffic:

```bash
server {
    listen 80;

    # Laravel
    location / {
        proxy_pass http://localhost:8000; # Laravel
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
        proxy_set_header Host $host;
        proxy_cache_bypass $http_upgrade;
    }

    # Node.js
    location /nodeapp {
        proxy_pass http://localhost:3000; # Node.js
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
        proxy_set_header Host $host;
        proxy_cache_bypass $http_upgrade;
    }
}
```

- Save the file and restart Nginx:

```bash
  sudo nginx -t
  sudo systemctl restart nginx
```

#### 7. **Start the Servers**

- Laravel: Start the Laravel server on port 8000.

```bash
php artisan serve --host=0.0.0.0 --port=8000
```

- Node.js: Start the Node.js server using PM2 for process management.

```bash
cd /var/www/node-backend
pm2 start index.js --name node-backend
```

<br><br>

<!-- Unit Testing -->
<img src="./readme/title9.svg"/>

### Precision in Development: Harnessing the Power of Unit Testing:

- In this project, unit testing was implemented using Laravel's built-in testing tools along with PHPUnit. PHPUnit was installed via `composer require --dev phpunit/phpunit` to provide a robust testing framework. Model factories were created to generate consistent test data, ensuring comprehensive coverage across various scenarios.

- The testing focused on key areas such as controller actions, API endpoints, file uploads/downloads, and middleware. Assertions like `assertJson`, `assertTrue`, and `assertStatus` were used to validate responses, while database checks were done with `assertDatabaseHas` to ensure data integrity.

##### Here is the result of the tests

<img src="./readme/demo/Unit_testing.png">
<br><br>

<!-- How to run -->
<img src="./readme/title10.svg"/>
<br><br>

> To set up VEDU locally, follow these steps:

### Prerequisites

- npm

```sh
  npm install npm@latest -g
```

- Download [composer](https://getcomposer.org/download/)
- Download [php](https://windows.php.net/download/)

### Installation

1. Get a free Pusher Key at channels at [Pusher](https://dashboard.pusher.com/)
2. Get a free GetStream key at Apps > video & audio > Overview at [getstream](https://dashboard.getstream.io/app)
3. Clone the repo

```bash
   git clone --recurse-submodules https://github.com/Ali-Rhayem/VEDU.git
```

4. Setup frontend

- open the terminal and navigate to front end directory

```bash
cd vedu-frontend/vedu-frontend
```

- run npm install from vedu-frontend directory

```sh
npm install
```

- Then go to .env.example file, rename it to .env and edit it as shown.

```.env
REACT_APP_SECRET_KEY: Secret key for your React app (can be a UUID or random string)
PUSHER_APP_ID: The Pusher App ID from your Pusher dashboard
REACT_APP_PUSHER_KEY: The Pusher key from your Pusher dashboard
REACT_APP_PUSHER_CLUSTER: The Pusher cluster from your Pusher dashboard
PUSHER_APP_SECRET: The secret key for Pusher from your Pusher dashboard
REACT_APP_STREAM_API_KEY: The API key for GetStream
REACT_APP_STREAM_API_SECRET: The secret for GetStream API
```

- If the server is no longer on aws then use

```.env
REACT_APP_API_BASE_URL_LOCAL:http://127.0.0.1:8000
```

5. Setup the laravel backend. (In case the website is no longer on aws or if you want to test it)

- open the terminal and navigate to backend directory

```bash
cd vedu-backend/vedu-backend
```

- run composer install from vedu-backend directory

```sh
composer install
```

- Then go to .env.example file, rename it to .env populate the values.

```.env
DB_DATABASE=VEDU
JWT_SECRET="Your Secret JWT key (Can be what ever you want)"
PUSHER_APP_ID: The Pusher App ID from your Pusher dashboard
REACT_APP_PUSHER_KEY: The Pusher key from your Pusher dashboard
REACT_APP_PUSHER_CLUSTER: The Pusher cluster from your Pusher dashboard
PUSHER_APP_SECRET: The secret key for Pusher from your Pusher dashboard
```

- and add the openai key

```.env
OPENAI_API_KEY=YOUR-OPENAI-KEY
```

- then to migrate the database run :

```bash
php artisan migrate
```

- and type y if you havent created the database yet

6. Setup the node backend. (In case the website is no longer on aws or if you want to test it)

- open the terminal and navigate to node backend directory

```bash
cd vedu-backend-node
```

- run npm install from vedu-backend-node directory

```sh
npm install
```

- Then add the .env file and add to it the openAi key

```.env
OPENAI_API_KEY=YOUR-OPENAI-KEY
```

7. Setup your electron

- open the terminal and navigate to admin directory

```bash
cd vedu-backend/vedu-backend
```

- run npm install from vedu-admin directory

```sh
npm install
```

8. Now all left is to run the project.

- From vedu-frontend directory open terminal and run

```sh
npm start
```

- From admin directory open terminal and run

```sh
npm start
```

- From vedu-backend directory open terminal and run (if you want to use it locally)

```sh
php artisan serve
```

- From node backend directory open terminal and run

```sh
npm start
```

Now VEDU is up and running, enjoy.
