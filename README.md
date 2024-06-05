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

### 1. Run Rails Server

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

## Production Deployment

### Frontend Deployment

#### 1. Configure Environment

```bash
VITE_WS_URL=wss://yourdomain.com/cable
VITE_API_URL=https://yourdomain.com
```

### Backend Deployment

#### 1. Configure Production Environment

Make sure your config/environments/production.rb is configured properly. Specifically, ensure Action Cable is set up for your production server:

```ruby
config.action_cable.allowed_request_origins = [ "https://yourdomain.com" ]
```

#### 2. Rails Credentials

This will open the credentials file in the Nano editor. save this master key for later.

```bash
EDITOR="nano" rails credentials:edit
```

#### 3. Configure environment variables

1. Set RAILS_MASTER_KEY to your master key.
2. Set REDIS_URL.

## Deployed app

1. Deployed frontend using vercel [Click Here](https://chat-client-delta-five.vercel.app/)
2. Deployed backend using render [Click Here](https://backend-chat-8kqi.onrender.com)

## Additional References

1. [Go rails documentation](https://gorails.com/)
2. [React documentation](https://react.dev/)
3. [Vite documentation](https://vitejs.dev/)
4. [Render Rails Documentation](https://docs.render.com/deploy-rails)
5. [Vercel Documentation](https://vercel.com/docs/frameworks/vite)
