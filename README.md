# Food Web App Project

Welcome to our Food Web App! This project offers various features for users to buy food products online. Below, you'll find a summary of what this app includes and how it works.

## Features

- **User Functionalities:**
  - **Buy Food Products:** Browse and purchase a variety of food items.
  - **Shopping Cart:** Add items to your cart and view them before purchasing.
  - **Order:** Place orders for the items in your cart.
  - **Payment Integration:** Pay securely through integrated payment methods.

- **Admin Functionalities:**
  - **Admin Dashboard:** Manage products, orders, and users from an easy-to-use admin interface.

## Technologies Used

- **Frontend:**
  - **Next.js:** A React framework for building fast web applications.
  - **Tailwind CSS:** A utility-first CSS framework for styling.
  - **DaisyUI:** A UI component library built on Tailwind CSS.

- **Backend:**
  - **Node.js:** JavaScript runtime for server-side programming.
  - **Express.js:** A web application framework for Node.js.
  - **Mongoose:** An Object Data Modeling (ODM) library for MongoDB and Node.js.

- **Security:**
  - **Password Hashing:** We use `bcrypt` to securely hash and store passwords in the database.
  - **JWT Authentication:** We use JSON Web Tokens (JWT) to provide secure login and sign-up functionality.

  - **How to use bcrypt:**
  bcrypt.genSalt(10)  // This function is used to generate unique salt and further we integrate this salt into actual user password while we hash the password so as that password become unique even if user input is same as before.

  bcrypt.hash(userPassword, salt) // This function is used to hash the password by integrating unique salt with user password and this is the main function which actually generates hash.

  bcrypt.compare(userInputPassword, storedHashedPassword) // This function is used at login time, when user try to login user enter is password that time user enter password is in plain text so it is not possible to compare plain text password with hash password which is stored in database so that time we have to use comapare function which compares plain text password with hash password. 

## How It Works

1. **Users:** Can browse food products, add them to their cart, and place orders. They can securely sign up and log in using JWT authentication.
2. **Admin:** Can manage the products, view orders, and oversee user activities through a dedicated admin interface.
3. **Security:** All passwords are hashed before storing in the database, ensuring they are kept safe. JWT tokens are used to authenticate users securely.

## Getting Started

To get started with the project, clone the repository and follow the setup instructions in the `README.md` file.
