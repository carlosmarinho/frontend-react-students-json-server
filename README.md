# Installation

Run the following commands

- Clone the application from https://github.com/carlosmarinho/frontend-react-students-json-server.git

  ```
  git clone https://github.com/carlosmarinho/frontend-react-students-json-server.git
  ```

- Get into the discompacted folder

  ```
  cd frontend-react-students-json-server
  ```

- Run npm install to install the package dependancy

  ```
  npm install
  ```

- Run npm run start to start the application
  ```
  npm run start
  ```

The last command (npm run servers) will run the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

# Backend

For easier instalation we can use a npm package called json-server, for a full backend features try to install the same backend of this application https://github.com/carlosmarinho/node-express-sequelize-react-students. If you want to follow the easier backend setup just follow bellows instructions, else follow the repo mentioned above.

- Get into the application folder

  ```
  cd frontend-react-students-json-server
  ```

- First we need to npm install to have the json-server that we are going to use our apis to be available on port 3001

  ```
  npm install -g json-server
  ```

- To run only the backend run npm run jsonserver as bellow

  ```
  json-server db.json -p 5000 --routes routes.json
  ```

# GIT LOG of this project

This project is a fork from https://github.com/carlosmarinho/node-express-sequelize-react-students, so if you want to see all the commits just get into this repository and see the full log there.

# Tecnologies used

- React
- Hooks
- Redux
- Redux Thunk
- Typescript
- CSS in JS (Styled Components)
- Jest
- React Testing Library
- json-server

# About the application

## Development

I started developing the application and decided to use redux, styled components and a bit of TDD with React Testing Library and Jest, but i stopped and finished the application with a lot of testing missing.

I decided to use all those thechnology, then you could have a good idea how can i develop a real application.

## Refactories (@todo)

### Templates, layouts and ContextApi

- Use ContextApi to update the current template.
- I created only one layouts with two columns but the application is designed to easily include others layouts, so the next layout update is to create another layout with only one column and the content.
- When change template, in the top menu, we have to change the colors from the whole site(left, right and content) according to the template colors.

### CSS styled components

- Take a look at the components to understand the need to separate the css from the component. We can decide if we are going to put all styled in separeted file or if we are going to separete only if there is a lot of style in the component.

### Test

- Increase the test coverage of the application

### Items (Student, Teacher - CRUD)

- Create the student pages and its components(CRUD) and link the top menu of students with it's components
- Create the teacher pages and its components(CRUD) and link the top menu of teachers with it's components

### Login

- We have the need to create a login for student and teachers, when the teachers login they have permission to change the current score in the right column

## Testing

- I started developing the application using TDD, but as it wasn't required and i want to speed things up, i stoped and there is a necessity to do some more testing.
- It will be created a folter test in the current dir of the component.
  - In this version we just have test on the folder /src/components/Students
- To run the test run `npm run test`
