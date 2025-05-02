# GateDrop

**GateDrop** is a web app that lets musicians trade SoundCloud engagement (likes, reposts, follows) for free music downloads. Users must complete a chosen engagement action before unlocking the download link.

## Features

- SoundCloud OAuth login for musicians and listeners  
- Upload a file and create a gated download link  
- Pull metadata (title, artist, cover) from SoundCloud links  
- Set required actions (like, repost, follow) before download unlocks  
- Musician dashboard with track stats  
- Cloud storage integration for hosting files  

## Demo

[Live Site](https://gatedrop.xyz) — *coming soon*

## Tech Stack

- Frontend: React, Tailwind, React Router  
- Backend: Node.js, Express, Prisma  
- Database: PostgreSQL  
- Auth: SoundCloud OAuth  
- File Storage: Cloudinary (or Backblaze)  
- Deployment: Vercel (frontend), Railway (backend)

## Getting Started

### Prerequisites

- Node.js
- PostgreSQL
- SoundCloud developer account

### Setup

```bash
git clone https://github.com/yourusername/gatedrop.git
cd gatedrop
```

#### Frontend

```bash
cd frontend
npm install
npm run dev
```

#### Backend

```bash
cd backend
npm install
npx prisma generate
npm run dev
```

### Environment Variables

Create `.env` files in both `frontend` and `backend` with required values:

**Backend/.env**

```
DATABASE_URL=postgresql://...
SOUNDCLOUD_CLIENT_ID=...
SOUNDCLOUD_CLIENT_SECRET=...
JWT_SECRET=...
CLOUDINARY_API_KEY=...
...
```

## License

MIT