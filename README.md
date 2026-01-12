# Phreddit
Phreddit is a full-stack Reddit clone. Phreddit employs the MERN stack (MongoDB, Express.js, React, Node.js) and it is complete with user accounts and secure authentication (bcrypt), subreddit and post creation, a voting/karma mechanism, and role-based privileges (user vs moderator vs admin).
## Running Instructions
- Make sure nodejs is installed. If it's not, install [here](https://nodejs.org/en/download)
- Make sure mongoDB is installed. If it's not, install the [community edition](https://www.mongodb.com/docs/manual/administration/install-community/)
- Run all commands in terminal
- In a terminal window, in the root directory, run **`$ npm i`**.
- In a new terminal window, navigate to the client directory (**`$ cd client`**), then run **`$ npm i`**. Finally, run **`$ npm start`**
- In a new terminal window, run **`$ mongod`**. Note: if you're using macOS with the package manager Homebrew, you may have to use **`$ brew services start mongodb-community@<version_number>`** instead.
- In a new terminal window, navigate to the server directory (**`$ cd server`**), then run **`$ npm i`**. Run **`$ npm run start`** to start the server. In a new terminal in the server directory, run **`$ npm run initDB`** to initialize the database with some initial data, including the administrator account with email: admin@admin.com, displayName: ADMIN, password: password123. Alternatively, to define your own admin account you can run **`$ node init.js mongodb://127.0.0.1:27017/phreddit <admin_email> <admin_displayName> <admin_password>`**. Both will initialize the database with default data.
- To run tests, navigate to the root directory and run **`$ npm test`**
