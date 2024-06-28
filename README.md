Form Recreation Project
This project is a form recreation application developed using the following technologies:

Frontend: React JS (version 18), React Bootstrap, CSS3
Backend: Node.js with Express.js, MongoDB for the database
API Integration: Axios
Testing: Postman
Deliverables
Source Code: GitHub Repository
Deployed Application: The frontend is deployed on Netlify. Access the application here.
Instructions
Setup and Run Locally
Frontend
Navigate to the frontend directory:

bash
Copy code
cd frontend
Install frontend dependencies:

bash
Copy code
npm install
Run the frontend application:

bash
Copy code
npm start
Backend
Navigate to the backend directory:

bash
Copy code
cd backend
Install backend dependencies:

bash
Copy code
npm install
Configure environment variables:
Create a .env file in the backend directory with the following content:

bash
Copy code
MONGO_URI=mongodb+srv://halaswamyg07:Milky@1234@cluster0.mongodb.net/myFirstDatabase?retryWrites=true&w=majority
PORT=5000
Run the backend server:

bash
Copy code
node index.js
Running Both Frontend and Backend Simultaneously
Install concurrently to run both servers simultaneously:

bash
Copy code
npm install concurrently --save-dev
Add a script to your root package.json to run both frontend and backend:

json
Copy code
"scripts": {
  "start": "concurrently \"cd frontend && npm start\" \"cd backend && node index.js\""
}
Run the application:

bash
Copy code
npm start
Access the Application
Open your browser and go to http://localhost:3000 to access the frontend locally.
For the deployed version, visit https://vyzen1.netlify.app/.
Design Choices and Features
React JS: Chosen for its component-based architecture, making it easier to manage and maintain the UI.
React Bootstrap: Used for a responsive and modern UI design.
Axios: Simplifies HTTP requests and API integration.
MongoDB: NoSQL database chosen for its flexibility in handling the form data.
Node.js with Express.js: Provides a robust backend framework.
Note
The project was intended to be deployed on the AWS Cloud, but I am currently unable to proceed with the deployment due to the requirement of a credit card for setting up an AWS account. I have also attempted to use Netlify for hosting the frontend and Vercel for the backend. Unfortunately, Vercel's read-only file system prevents uploading images or documents. Therefore, the backend is deployed locally for now. Please use the provided MongoDB credentials to test and further process the application.

MongoDB Credentials:

Username: halaswamyg07@gmail.com
Password: Milky@1234
