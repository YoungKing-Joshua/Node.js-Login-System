
# Node.js Login System
In this project, I created a web application using Node.js and Express, implementing user authentication sand authorization.

### Approach:

I built a web application that allows users to register and log in. The application includes authentication using passport.js and bcrypt for securely storing user passwords. The user registration form collects the user's full name, email address, and password. Upon registration, the password is hashed using bcrypt and stored in the database. For login functionality, the application compares the hashed password with the user's input using bcrypt to verify the login credentials.

### Implementation:

To implement user authentication and authorization, I utilized the following libraries and techniques:

1. `express`: A fast and minimalist web framework for Node.js.
2. `bcrypt`: A library for hashing passwords securely.
3. `passport`: An authentication middleware for Node.js that provides various authentication strategies.
4. `express-flash`: A middleware for displaying flash messages.
5. `express-session`: A middleware for managing user sessions.
6. `method-override`: A middleware for handling HTTP methods other than GET and POST.

I structured the application using the Model-View-Controller (MVC) pattern. The `server.js` file handles the server setup, routes, and middleware configurations. The `passport-config.js` file sets up the local authentication strategy using passport.js.

The `views` directory contains the HTML templates for the login and registration pages, implemented using Embedded JavaScript (EJS) templates. The `index.ejs` file represents the user's dashboard after successful login.

### Data Storage:

In this task, I stored user data in an in-memory array for demonstration purposes. However, in a real-world scenario, it is recommended to store user data in a reliable database, such as PostgreSQL. Using a database ensures data persistence and allows for more robust data management, scalability, and data security.

To switch to a database like PostgreSQL, you can use libraries like `pg-promise` or `sequelize` to handle the database interactions within the Node.js application. The database connection details (such as hostname, username, password, and database name) can be stored as environment variables to ensure security.

### How to Run the Application:

1. Clone this repository to your local machine.
2. Ensure you have Node.js and npm (Node Package Manager) installed.
3. Navigate to the project folder and run the following command to install the required dependencies:

```
npm install
```

4. To start the application, run the following command:

```
node server.js
```

5. The application will be running on `http://localhost:3000`.

### Important Note:

- This application is for demonstration purposes and not intended for production use. It is solely meant to showcase my understanding of building user authentication and authorization in a Node.js web application.

[Joshua Dei-Alorse]