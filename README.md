# SceneVault-jvks

A discovery platform for writers to find and browse scene excerpts by genre and situation for inspiration, plus tools to map out your own stories.

## Features

- 🔍 **Scene Discovery**: Search and filter writing scenes by genre, situation, and keywords
- 📚 **Story Mapping**: Organize your stories with character tracking, settings, plot points, and notes
- 🎨 **Coffee Theme**: Warm, writer-friendly interface with brown and beige tones
- 💾 **Persistent Storage**: PostgreSQL database for reliable data storage
- 🌙 **Dark/Light Mode**: Toggle between themes for comfortable writing sessions

## Tech Stack

- **Frontend**: React 18, TypeScript, Tailwind CSS, shadcn/ui
- **Backend**: Node.js, Express, TypeScript
- **Database**: PostgreSQL with Drizzle ORM
- **Build Tool**: Vite

## Deployment Options

### Vercel (Recommended)
1. Connect your GitHub repository to Vercel
2. Set environment variable: `DATABASE_URL`
3. Deploy automatically

### Netlify
1. Connect your GitHub repository to Netlify
2. Set environment variable: `DATABASE_URL`
3. Build command: `npm run build`
4. Publish directory: `dist/public`

### Railway
1. Connect your GitHub repository to Railway
2. Set environment variable: `DATABASE_URL`
3. Deploy automatically

## Environment Variables

```
DATABASE_URL=your_postgresql_connection_string
NODE_ENV=production
```

## Local Development

```bash
# Install dependencies
npm install

# Set up database
npm run db:push

# Start development server
npm run dev
```

## Database Setup

The app uses PostgreSQL. You can get a free database from:
- **Neon** (recommended): https://neon.tech
- **Supabase**: https://supabase.com
- **PlanetScale**: https://planetscale.com

Copy your database URL to the `DATABASE_URL` environment variable.

## Project Structure

```
├── client/          # React frontend
├── server/          # Express backend
├── shared/          # Shared types and schemas
├── vercel.json      # Vercel deployment config
├── netlify.toml     # Netlify deployment config
└── package.json     # Dependencies and scripts
```

## Support

This project is ready for deployment on any modern hosting platform that supports Node.js and PostgreSQL.