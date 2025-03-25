# video-streaming 
MERN Video Streaming is a cutting-edge, open-source platform for video streaming, offering a comprehensive, full-stack solution utilizing the latest MERN stack technologies. With MERN Video Streaming, users can easily upload, manage, and stream videos on demand, providing a seamless experience. This project features a video processing capability that provides real-time notifications upon completion.

The backend is comprised of three services, utilizing Redis messaging for communication. These include an API server, a video conversion service, and an HTTP server serving HLS video files. On the client side, the project uses create-react-app and MUI library, along with socket.io-client and React Context.

Backend Services
API Server
The API server is an Expressjs app that uses Joi, Multer, BullMQ, Socket.io, and MongoDB driver. The server communicates with Redis to process and store data, and uses MongoDB as the primary database. The database and Redis are spun up via the docker-compose command.

Video Conversion Service
The video conversion service is a node process that is responsible for converting videos and communicating with Redis via the BullMQ library. The service is not exposed to any HTTP port.

HTTP Server
The HTTP server is a plain and simple server that serves HLS video files.

Frontend app
The client app is based on create-react-app and MUI library. It uses socket.io-client and React Context to communicate with the API server and display the video content.

Prerequisites
To get started with MERN Video Streaming, you will need to have the following software installed on your local machine:

Node.js
Docker
Docker Compose
Built with Open-Source Technologies
MERN Video Streaming has been built with the following open-source technologies:

MongoDB - A document-based database used to store user and video data
Express - A Node.js web application framework used for the server-side of the application
React - A JavaScript library for building user interfaces used for the client-side of the application
Node.js - A JavaScript runtime environment used to run the server-side code
