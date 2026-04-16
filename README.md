# UGC.AI - AI Video Generation Platform

Welcome to the **UGC.AI** repository! This is an advanced AI-powered video generation platform built to streamline the creation of user-generated content using cutting-edge AI models, complete with a tiered subscription system.

## 🚀 Features

- **Automated Video Generation:** Leverage powerful AI APIs (Google GenAI, Magic Hour) to automatically generate compelling video content.
- **Subscription Tiers:** Integrated credit-based feature gating (Free, Pro, Premium) to manage usage and offer premium features.
- **Secure Authentication:** User authentication and management is handled seamlessly with [Clerk](https://clerk.com/).
- **Media Processing & Storage:** Robust file handling using Cloudinary for image/video hosting and `fluent-ffmpeg` for advanced media processing.
- **Modern UI/UX:** A beautiful, responsive frontend built with React, Tailwind CSS, and Framer motion animations.

## 🛠️ Tech Stack

### Frontend (Client)
- **Framework:** [React](https://react.dev/) + [Vite](https://vitejs.dev/)
- **Styling:** [Tailwind CSS](https://tailwindcss.com/)
- **Animations:** [Framer Motion](https://www.framer.com/motion/)
- **Authentication:** Clerk React SDK
- **Routing:** React Router DOM

### Backend (Server)
- **Runtime:** [Node.js](https://nodejs.org/)
- **Framework:** [Express.js](https://expressjs.com/)
- **Database:** PostgreSQL (with [Prisma](https://www.prisma.io/) ORM)
- **Cloud Storage:** Cloudinary
- **AI Integrations:** Google GenAI SDK, Magic Hour API
- **Media Processing:** FFmpeg (`fluent-ffmpeg`, `ffmpeg-static`)

## 📦 Project Structure

The repository is organized into a monorepo-style structure:

- `/client` - Contains the React frontend application.
- `/server` - Contains the Node.js/Express backend application and Prisma schema.

## 🚦 Getting Started

### Prerequisites
- Node.js (v18+)
- PostgreSQL Database
- API Keys for Clerk, Cloudinary, Google GenAI, and Magic Hour.

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd "SaaS Project"
   ```

2. **Install Client Dependencies:**
   ```bash
   cd client
   npm install
   ```

3. **Install Server Dependencies:**
   ```bash
   cd ../server
   npm install
   ```

4. **Environment Variables:**
   - Set up your `.env` files in both the `client` and `server` directories with the required API keys and database URLs.

5. **Database Setup:**
   - In the `server` directory, run Prisma migrations to initialize your database:
   ```bash
   npx prisma migrate dev
   ```

### Running the Application Locally

You can run both the client and server concurrently:

**Start the Server:**
```bash
cd server
npm run server
```

**Start the Client:**
```bash
cd client
npm run dev
```

## 📄 License

This project is licensed under the ISC License.
