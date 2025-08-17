

# MERN Ecommerce

## Description

An ecommerce store built with the MERN stack that utilizes third-party APIs. This ecommerce store supports three main flows:

1. **Buyers** – Browse the store categories, products, and brands.
2. **Sellers/Merchants** – Manage their own brand components.
3. **Admins** – Manage and control the entire store.

### Features

* **Node.js** for the backend environment.
* **Express** middleware to handle requests and routes.
* **Mongoose** schemas to model application data.
* **React** for UI components.
* **Redux** to manage application state.
* **Redux Thunk** middleware for asynchronous Redux actions.

## Docker Guide

To run this project locally using Docker Compose:

1. Clone the repository:

```bash
git clone <your-repo-url>
```

2. Edit the `dockercompose.yml` file and update the values for `MONGO_URI` and `JWT_SECRET`.
3. Start Docker Compose:

```bash
docker-compose build
docker-compose up
```

## Database Seed

* The seed command creates an admin user in the database.
* Email and password are passed as arguments:

```bash
npm run seed:db [email@example.com] [password]
```

* For more details, see `server/utils/seed.js`.

## Install

In the project root, run:

```bash
npm install
```

This will install dependencies in both `client` and `server`.

Or manually:

```bash
git clone <your-repo-url>
cd project
npm install
```

## ENV Setup

Create `.env` files for both client and server. See:

* `client/.env.example`
* `server/.env.example`

## Start Development

```bash
npm run dev
```

## Languages & Tools

* [Node.js](https://nodejs.org/en/)
* [Express](https://expressjs.com/)
* [Mongoose](https://mongoosejs.com/)
* [React](https://reactjs.org/)
* [Webpack](https://webpack.js.org/)

### Code Formatter

1. Add a `.vscode` directory.
2. Create a `settings.json` file inside `.vscode`.
3. Install **Prettier – Code Formatter** in VSCode.
4. Add:

```json
{
  "editor.formatOnSave": true,
  "prettier.singleQuote": true,
  "prettier.arrowParens": "avoid",
  "prettier.jsxSingleQuote": true,
  "prettier.trailingComma": "none",
  "javascript.preferences.quoteStyle": "single"
}
```


# **Made by Suleiman Abdulkadir**

