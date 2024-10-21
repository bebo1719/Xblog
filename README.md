Xblog
Description
Xblog is a CMS-style blog site where developers can publish their articles, blog posts, thoughts, and opinions. Built using the Model-View-Controller (MVC) architecture, this application allows users to sign up, log in, create, update, and delete their blog posts. Additionally, users can interact with the platform by commenting on blog posts.

The application is designed with a responsive front-end, a robust back-end using Node.js, Express.js, Sequelize ORM, and PostgreSQL for data storage.

Table of Contents
Installation
Usage
Features
Technologies Used
Screenshots
License
Contributing
Questions
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/xblog.git
Navigate into the directory:

bash
Copy code
cd xblog
Install the dependencies:

bash
Copy code
npm install
Create a .env file in the root of your project with the following variables:

arduino
Copy code
DB_NAME='your-database-name'
DB_USER='your-database-username'
DB_PASSWORD='your-database-password'
DB_HOST='localhost'
SECRET='your-secret-session-key'
Create the database and tables using Sequelize:

bash
Copy code
npx sequelize db:create
npx sequelize db:migrate
(Optional) Seed the database with some initial data:

bash
Copy code
npm run seed
Start the application:

bash
Copy code
npm start
Usage
Open your browser and navigate to http://localhost:3001 to view the Xblog homepage.
Sign up or log in to start creating blog posts.
View, edit, and delete your blog posts through the dashboard.
Comment on posts created by other users.
Features
User Authentication: Users can sign up, log in, and log out securely using session-based authentication.
Blog Post Management: Users can create, update, and delete their blog posts.
Commenting System: Users can comment on blog posts.
Responsive UI: The site is responsive, ensuring accessibility across various devices.
Handlebars Templating: Views are rendered using Handlebars.js, with dynamic routing and content management.
MVC Architecture: The application follows the MVC design pattern, separating concerns between data (models), user interface (views), and logic (controllers).
Technologies Used
Node.js: Server-side JavaScript runtime.
Express.js: Web application framework for Node.js.
Sequelize: ORM for PostgreSQL, providing an interface to interact with the database.
PostgreSQL: Database management system.
Handlebars.js: Templating engine used for dynamic HTML rendering.
bcrypt: Password hashing for authentication.
express-session: Session middleware for session management.
dotenv: Environment variable management.
connect-session-sequelize: Session storage in Sequelize.
Screenshots
Here are some screenshots showcasing the different features of Xblog:

Homepage

Dashboard

Create Post

License
This project is licensed under the MIT License. See the LICENSE file for details.

Contributing
If you'd like to contribute to Xblog, feel free to submit a pull request. Please ensure that your code follows the style guidelines and passes all tests.

Fork the repository.
Create a new branch: git checkout -b feature-branch-name.
Make your changes and commit them: git commit -m 'Add some feature'.
Push to the branch: git push origin feature-branch-name.
Submit a pull request.
