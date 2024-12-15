# Harsha's Social Media App

A full-stack social media app built with Node, Express, Angular, and MySQL. This project allows users to share posts, comment on posts, and manage profiles, showcasing a simple and scalable architecture.


## Tech Stack

- **Frontend:** Angular
- **Backend:** NodeJS, ExpressJS
- **Database:** MySQL (for database)

Run following command:

>npm install

That installs dependencies requierd in node_modules folder.
___

## CLIENT

Start client:
>npm start

link: https://localhost:4200

After you are done developing client, use following command to make build so you can try it on your local network.

>npm run build

That compiles all client code to one html and four js files that our server is going to serve.

And after build new changes will be availible on you local network.

___

## SERVER
Start server:

Link will be logged in console after you start it, that will look like next two following lines.

Server starting...

Listening at 100.103.0.120:3000

>npm run serve

After starting server, you can visit app on https://localhost:4200 from Angular server that has proxy to our coded server.

___

## DATABASE
Database is MySQL, and for this application I used XAMP. Install it and create database named "social_media". 