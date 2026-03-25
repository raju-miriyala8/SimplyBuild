# SimplyBuild

SimplyBuild is a full-stack MERN application that lets users describe a web app idea in natural language and generate working frontend code with AI.

The app includes user authentication, project management, an AI chat-based builder, live preview, and editable generated code. Users can create a project from an idea, iterate through prompts, preview the result, and download the generated output.

## Features

- User signup and login with JWT authentication
- Dashboard for creating, opening, and deleting projects
- Chat-driven project generation workflow
- Live preview for generated apps
- Editable code view for generated output
- AI-powered code generation using Gemini

## Tech Stack

- Frontend: React, Vite, React Router, Axios
- Backend: Node.js, Express
- Database: MongoDB with Mongoose
- Authentication: JWT, bcryptjs
- AI: Google Gemini API

## Project Structure

```text
client/   React frontend
server/   Express backend
```

## Getting Started

### 1. Install dependencies

```bash
cd client
npm install

cd ../server
npm install
```

### 2. Configure environment variables

Create a `.env` file inside `server/` and add your values:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=7d
GEMINI_API_KEY=your_gemini_api_key
CLIENT_URL=http://localhost:5173
```

### 3. Run the app

Backend:

```bash
cd server
npm run dev
```

Frontend:

```bash
cd client
npm run dev
```

## Usage

- Sign up or log in
- Open the dashboard
- Click `New Project`
- Describe your app idea in the builder chat
- Review the generated preview and code
- Refine with more prompts or download the result

## Notes

- Do not commit `.env` files or API keys
- Generated output depends on your Gemini API configuration

