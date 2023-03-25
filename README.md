

<h1 align="center">
  <br>
  <a href="http://www.amitmerchant.com/electron-markdownify"><img src="https://iili.io/HN7PPyl.md.jpg" alt="Shockbyte Birdhouses logo" width="200"></a>
  <br>
  Shockbyte Birdhouses Server
  <br>
</h1>

<h4 align="center">An API for managing birdhouses and their residencies made in <a href="https://nestjs.com/" target="_blank">NestJS</a>.</h4>



<p align="center">
  <a href="#how-to-use">How To Use</a> •
  <a href="#thought-process">Thought process</a> •
  <a href="#credits">Credits</a> •
  <a href="#related">Related</a> •
  <a href="#license">License</a> 


</p>

![screenshot](https://iili.io/HN75NY7.gif)

## How To Use

To clone and run this application, you'll need [Git](https://git-scm.com), [Docker](https://www.docker.com/products/docker-desktop/) and [Node.js](https://nodejs.org/en/download/) (which comes with [npm](http://npmjs.com)) installed on your computer. From your command line:

```bash
# Clone this repository
$ git clone https://github.com/jontatan25/birdhouse-API

# Go into the repository / server folder
$ cd electron-markdownify
$ cd server

# Install dependencies
$ npm install

# Start the Docker container
$ docker-compose up -d birdhousedb

# Run the app
$ npm start
```
> **Note**
> If you're using Linux Bash for Windows, [see this guide](https://www.howtogeek.com/261575/how-to-run-graphical-linux-desktop-applications-from-windows-10s-bash-shell/) or use `node` from the command prompt.

• Once the app is running navigate to http://localhost:3000/api to see the full Documentation

## Thought process


1.  Setup the development environment: Install all the necessary tools and dependencies required for developing the project.
    
2.  Create the backend application using NestJS. Implement the necessary endpoints for communication with the birdhouses, according to the BIRD standard. Create House entity.
    
3.  Create a Service for the BirdsHouses, and implement it with the endpoints, move the methods to the new service.
    
4.  Create a Module for the BirdsHouses, and implement it. 
    
5.  Now that the core structure has been stablished, create DTOs
6.  Validate the data: implement ValidationPipe for the app and class-validator for the DTOs
7. Time to implement the DB, must be relational and easy to deploy so that the person who reviews can easily replicate the DB, research... TypeOrm, Postgres + Docker.
8. Create entities and relations, and update the Types according to it
9. Update methods to work with the DB
10. Auth is required for the routes that update a Birdhouse, lets create a middleware that will take of that.
11. Admins require new endpoints,methods and a different Auth method, Create routes with methods and The new middleware  
12. The interactions with the API must be logged, lets implement a console.log and if I have some extra time after the frond-end is completed, implement a Logger.
13. routes are complete, Let's see what can we refactor to make it more organized and make sure that everything is where it should be.
14. A few days later... Yey ! Front-end was completed. let's implement Winston, Clean the code, make sure that there is no boilerplate or unused files.
15. Create the Documentation, 

## Credits

This software uses the following open source packages:

- [Nestjs](https://nestjs.com/)
- [Node.js](https://nodejs.org/)
- [node-postgres](https://github.com/brianc/node-postgres)
- [typeorm](https://typeorm.io/)
- [uuid](https://github.com/uuidjs/uuid)
- [winston](https://github.com/winstonjs/winston)

## Related

[Shockbyte](https://shockbyte.com/) - The best game server provider.

## License

MIT

---

> GitHub [@jontatan25](https://github.com/jontatan25) &nbsp;&middot;&nbsp;


