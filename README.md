# Take-Home Project: Real-time Task Board

## Overview

Build a simple real-time task board where users can create and move tasks between columns. Multiple users should see updates instantly via WebSockets.

**Time Limit:** 2 hours

**Required:** Must be deployed and accessible via URL

## Tech Stack

- **Frontend:** Next.js + TypeScript
- **Backend:** Node.js or Go with WebSockets
- **Deployment:** Your choice (Vercel, Railway, Render, fly.io, etc.)

## Required Features

1. **4 columns:** "To Do", "In Progress", "Done", "Unsure"
2. **Create tasks:** Simple form to add a task with a title
3. **Move tasks:** Drag-and-drop OR buttons to move between columns
4. **Delete tasks:** Ability to remove tasks
5. **Database:** Connect to either **MongoDB** or **PostgreSQL** (your choice)
   - Tasks must persist across server restarts
   - Free tiers: MongoDB Atlas, Supabase, Neon, Railway, etc.
6. **Real-time sync:** All connected users see changes instantly via WebSockets
7. **Backend:** Must have a separate backend service (Node.js or Go)
8. **Deployed:** Both frontend and backend must be live and accessible

## Optional (if you have time)

- Edit task titles
- Simple authentication with better auth or a similar library
- Task descriptions or metadata

##

You can use any AI tool. However projects will be rated much harsher so abuse it.

## Evaluation

- Does it work? Can we test it live?
- A nice front end design is huge factor.
- Real-time functionality working correctly?
- Clean, readable code
- Deployment successful to a url

## Deadline & Submission

You have 2 hours from the time I sent you this.

Fork this repo and start a new branch to start your work. or just email your repo @ axel@rentbamboo.com


---

## Quick Start Commands

### Frontend (Next.js)
```bash
npx create-next-app@latest frontend --typescript --tailwind --app
cd frontend
npm install
npm run dev
```

### Backend - Node.js Option
```bash
mkdir backend && cd backend
npm init -y
npm install express ws cors dotenv
npm install --save-dev typescript @types/node @types/express @types/ws ts-node nodemon
npx tsc --init
```

### Backend - Go Option
```bash
mkdir backend && cd backend
go mod init taskboard-backend
go get github.com/gorilla/websocket
go get github.com/gorilla/mux
```
