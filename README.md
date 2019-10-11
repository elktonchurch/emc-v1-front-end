<a href="https://elktonmc.live/">
    <img src="./src/assets/emc-logo-wide.png" title="EMC Logo" width="200" align="right">
</a>

# The Elkton Missionary Church (EMC) Web App

![MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)
![React](https://img.shields.io/badge/React-v16.9.0-blue.svg)
[![GitHub issues](https://img.shields.io/github/issues/elkton-mc/front-end)](https://github.com/elkton-mc/front-end/issues)
[![GitHub forks](https://img.shields.io/github/forks/elkton-mc/front-end)](https://github.com/elkton-mc/frontend/network)
[![GitHub stars](https://img.shields.io/github/stars/elkton-mc/front-end)](https://github.com/elkton-mc/frontend/stargazers)
[![Netlify Status](https://api.netlify.com/api/v1/badges/b5c4db1c-b10d-42c3-b157-3746edd9e81d/deploy-status)](https://elktonmc.live/)

## Project Overview

The EMC web app was built to serve Jesus Christ, through the Elkton Missionary Church, in its mission to make disciples that make disciples.

<br>

## Contributors

|                                                                                                               [Tico Thepsourinthone](https://hellotico.com)                                                                                                                |
| :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| [<img src="https://media.licdn.com/dms/image/C4E03AQGIjp9UmRoNXA/profile-displayphoto-shrink_200_200/0?e=1573084800&v=beta&t=p2pz2FMpiP7p40p6E2RHNglAjRz3HJI-W3vOUHAESuA" width= "110" height="auto" style="object-fit:cover; overflow:hidden;" />](https://hellotico.com) |
|                                                                                           [<img src="https://github.com/favicon.ico" width="25"> ](https://github.com/ticotheps)                                                                                           |
|                                                                         [ <img src="https://static.licdn.com/sc/h/al2o9zrvru7aqj8e1x2rzsrca" width="25"> ](https://www.linkedin.com/in/ticotheps/)                                                                         |

<br>
<br>

[EMC Web App Trello Board](https://trello.com/b/oRS2ZOGQ/emc-app)

<p align="center">
    <a href="https://trello.com/b/oRS2ZOGQ/emc-app">
        <img src="./src/assets/emc_trello.png" alt="EMC App Trello Board" width="500">
    </a>
</p>

<!-- [ENDRSD Release Canvas v1.0](https://www.notion.so/ENDRSD-v1-0-3e87edcf085e45dc993422f0668e0842)

<p align="center">
    <a href="https://www.notion.so/ENDRSD-v1-0-3e87edcf085e45dc993422f0668e0842">
        <img src="https://res.cloudinary.com/endrsd/image/upload/v1568019704/release_canvas_1_sm4hdq.png" alt="ENDRSD Notion document release canvas v1.0" width="500">
    </a>
</p> -->

<!-- ## Key Features

- Church members can create their own user accounts and passwords
- Users are able to login & logout to protect their contact information
- With proper credentials, users are able to view the contact information of other Church members

## Tech Stack

### Front end built using:

#### React.js, React Hooks, & Redux

- It comes with a good supply of documentation, tutorials, and training resources because of the well established community around it.
- The use of components allows for modularity, leading to faster and more efficient development.
- Components can house their own logic and controls.
- Testing with React.js is very straight-forward and comes with great documentation.

#### Front end deployed to [Netlify](https://elktonmc.live)

#### [Back end](https://github.com/elkton-mc/back-end) built using:

#### PostgreSQL

- PostgreSQL is a type of relational database that is open source and freely available for anyone to use.
- SQL databases have a reputation for being more reliable because they have been tried and tested longer than their NoSQL counterparts.
- The source code for PostgreSQL was developed by a large community that has created numerous online resources for support.
- The strongly-typed schemas with a SQL database leave very little room for errors.

#### Node.js

- Node.js offers easy scalability because it can handle a large number of simultaneous connections with high throughput.
- Using node.js allows developers who are familiar with JavaScript, to develop both the client-side and server-side applications using a single programming language.
- Node.js takes less time to learn because it utilizes an already popular client-side scripting language---JavaScript.
- Support for node.js is readily available because of the large and active community behind it.
- Node.js is able to take advantage of caching things within the application memory for faster load times.

#### Express.js

- Express.js makes web application development with node.js fast and easy.
- It is very easy to configure and customize express.js.
- Express.js allows you to create a REST API server.
- Allows you to define routes of your application based on HTTP methods and URLs.

#### Knex.js

- A SQL query builder that integrates well with a PostgreSQL database.
- Allows for 'migrations', which makes it easier to manage tables within the PostgreSQL database.
- It can create sequential files with timestamps and even manage table alterations.
- Allows for the creation of 'seeds', which can be used to consistently populate the database.

# Authentication

#### JSON Web Tokens

- A self-contained token which has authentication information, expiration information, and other user properties.
- JWTs don't have sessions to manage (stateless).
- No database table is required, which means fewer database queries.
- Can be used across multiple services.

#### Bcrypt.js

- Protects against 'rainbow table attacks'.
- Resistant to brute-force search attacks.

# API Server URLs

- [Local Server URL](https://localhost:5000/api/v1)
- [Staging Server URL](https://endrsd-api-staging.herokuapp.com/api/v1)
- [Production Server URL](https://endrsd-api.herokuapp.com/api/v1)

# API Endpoints

- GET `/api/v1/users/:userId`
- GET `/api/v1/tracks`
- GET `/api/v1/requirements`
- GET `api/v1/requirements/:requirementsId/steps`
- POST `/api/v1/users`
- POST `/api/v1/login`
- PUT `/api/v1/requirements/:requirementsId/steps`

# Environment Variables

In order for the app to function correctly, the user must set up their own environment variables. There should be a .env file containing the following:

    *  JWT_SECRET=<your-secret-here>
            -This can be any unique string of characters.

    *  REACT_APP_STAGE=staging
            -This must be included in the .env to utilize the staging database.

    *  REACT_APP_STAGE=production
            -This must be included in the .env to utilize the production database.

If no `REACT_APP_STAGE` environment variable is added to the `.env` file, the default local database on port 5000 will be utilized.

# Installation Instructions

After cloning this repo on to your local machine, use the package manager [yarn](https://yarnpkg.com/en/) to install all of the required dependencies for the ENDRSD app.

```bash
yarn install
```

When all of the proper dependencies have been installed, create a `.env` file that stores the `JWT_SECRET` and the `REACT_APP_STAGE` environment variables as shown above. This particular `.env` setup will allow you to immediately connect to the staging database instead of having to create a local database.

```bash
JWT_SECRET=<your-secret-here>
REACT_APP_STAGE=staging
```

Lastly, run `yarn start` to create a build on your local machine that can be viewed at `http://localhost:3000`.

```bash
yarn start
```

<p align="center">
    <img src="https://res.cloudinary.com/endrsd/image/upload/v1568018944/local_host_xpzo9l.png" alt="GIF walk-through" width="600">
</p>

## Other Scripts

    * format - formats code using 'Prettier' extension
    * build - creates a build of the application
    * start - starts the production server after a build is created
    * test - runs tests in **tests** directory
    * eject - copy the configuration files and dependencies into the project so you have full control over them -->

# Contributing

When contributing to this repository, please first discuss the change you wish to make via issue, email, or any other method with the owners of this repository before making a change.

Please note we have a [code of conduct](./CODE_OF_CONDUCT.md). Please follow it in all your interactions with the project.

## License

[MIT](https://choosealicense.com/licenses/mit/)

## Issue/Bug Request

**If you are having an issue with the existing project code, please submit a bug report under the following guidelines:**

- Check first to see if your issue has already been reported.
- Check to see if the issue has recently been fixed by attempting to reproduce the issue using the latest master branch in the repository.
- Create a live example of the problem.
- Submit a detailed bug report including your environment & browser, steps to reproduce the issue, actual and expected outcomes, where you believe the issue is originating from, and any potential solutions you have considered.

### Feature Requests

We would love to hear from you about new features which would improve this app and further the aims of our project. Please provide as much detail and information as possible to show us why you think your new feature should be implemented.

### Pull Requests

If you have developed a patch, bug fix, or new feature that would improve this app, please submit a pull request. It is best to communicate your ideas with the developers first before investing a great deal of time into a pull request to ensure that it will mesh smoothly with the project.

Remember that this project is licensed under the MIT license, and by submitting a pull request, you agree that your work will be, too.

#### Pull Request Guidelines

- Ensure any install or build dependencies are removed before the end of the layer when doing a build.
- Update the README.md with details of changes to the interface, including new plist variables, exposed ports, useful file locations and container parameters.
- Ensure that your code conforms to our existing code conventions and test coverage.
- Include the relevant issue number, if applicable.
- You may merge the Pull Request in once you have the sign-off of two other developers, or if you do not have permission to do that, you may request the second reviewer to merge it for you.

### Attribution

These contribution guidelines have been adapted from [this good-Contributing.md-template](https://gist.github.com/PurpleBooth/b24679402957c63ec426).

## Documentation

See [Backend Documentation](https://github.com/elkton-mc/back-end/blob/master/README.md) for details on the backend of our project.
