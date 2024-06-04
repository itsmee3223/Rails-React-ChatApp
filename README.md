# Simple Chat Application

This is a chat application built with Ruby on Rails and React, using Vite for the frontend bundling.

## Prerequisites

- Ruby 3.1.0
- Rails 7.0.4
- Node.js (latest version)
- Yarn or npm

## Installation

### 1. Clone the Repository
Clone the repository from GitHub:
```bash
git clone repo-link
cd project-name
```

### 2. Install Ruby Dependencies
```bash
bundle install
```

### 3. Install Node.js Frontend Dependencies
```bash
cd client
```
```bash
# Using npm
npm install

# or using yarn
yarn install
```

### 4. Running DB migration
```bash
rails db:migrate
```

## Running the Application

### 1.  Run Rails Server
Server will running on port 3000 in localhost or you can see in the terminal what port server is running
```bash
rails server
```

### 2. Run React Server
See in the terminal log what port is running and you can open the browser for the app
```bash
cd client

# Using npm
npm run dev

# or using yarn
yarn dev
```

## Additional References
1. [Go rails documentation](https://gorails.com/)
2. [React documentation](https://react.dev/)
3. [Vite documentation](https://vitejs.dev/)
