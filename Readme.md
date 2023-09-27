# Todo App as a Single Page Application

<img src="https://imgur.com/FJBGuEj.jpg" title="Todo App"/>

The SPA with 5 pages (routes):

- A Homepage to ask Signup or Signin to the application,
- Register page for users to register to be able to use the app,
- Login page for users to authenticated in the app to access private pages,
- A Dashboard page which shows authenticated/registered user todos and actions
- Notfound page

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

### Demo

Online Deployment of this project is available at [Todo App](https://tv2z-app.herokuapp.com/).

You can use below credentials to test pagination and search functions of the app. The database is populated by fakerjs library.



### Getting Started

To get started you can simply clone the repo and install the dependencies in the root folder


| Install |`npm install`                      |
| Run     |`npm run dev`                      |

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.



### Application

#### ES6 + Features

- Arrow Functions
- Template Literals
- Destructuring Assignment
- Block-Scoped Variables Let and Const
- async await with try/catch
- Spread operator
- Modules export/import
- New Built-In Methods
- Default Parameters

#### Libraries/Frameworks

- react: UI library
- react-router-dom: The router components of react
- redux react-redux: Global State Management framework
- redux-thunk: Middleware for async calls
- react-bootstrap: React integration for bootstrap css framework
- react-toastify: A library for react to have app level notification
- axios: to make HTTP requests
- nodejs: JS runtime for backend
- express: server/web framework for nodejs to create server
- express-validator: validator library for express framework
- mongoose: mongodb database library for nodejs
- bcryptjs: hashing library which is used to hash passwords in this project
- jsonwebtoken: JWT implementation library

#### Flow

##### Component Hierarchy

```
  App
│ │
│ ├── Navbar
│ │
│ ├── ToastContainer
│ │
│ ├── Homepage
│ │
│ ├── Register
│ │
│ ├── Login
│ │
│ ├── Notfound
│ │
│ ├── Dashboard
│ │ ├── PageSize
│ │ ├── Search
│ │ └── TodoList
          └── Todo
                 ├── FlexTable
                 │
                 ├── Modal
                 │
                 └── Pagination

```

##### Global State Flow

- auth: stores authentication states
- todo: stores todo states
- tag: stores todo tag states
- search: stores search states and results
- pagination: stores pagination states and items

```

#### Api Calls

1. Post - Register User

```
`../api/users`,

```

2. Post - Login User

```
`../api/auth`,

```

3. Get - Get todo tags

```
`../api/tags`,

```

4. Get/Post/Put/Delete Todos (Add/Update/Complete/Uncomplete/Delete/Get)

```
`../api/todos`,

```

##### NOTE: Local Storage

JWT token for authentication is stored in the local storage of the browser and added to header of the request by setAuthToken function.

### Author

- [salih18](https://github.com/salih18)
