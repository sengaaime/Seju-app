# Seju - Social Media App

A modern social media application built with Next.js, featuring real-time messaging, image sharing, and online status tracking.

## Features

- 🔐 **User Authentication** - Secure login/register system
- 📝 **Post Creation** - Share text and images with the community
- 💬 **Real-time Chat** - One-on-one messaging system
- 👥 **User Discovery** - Find and connect with other users
- 🟢 **Online Status** - See who's currently active
- ❤️ **Social Interactions** - Like and comment on posts
- 🔔 **Message Notifications** - Unread message badges
- 📱 **Responsive Design** - Works on all devices
- 🎨 **Modern UI** - Clean black and white theme

## Tech Stack

- **Frontend**: Next.js 14, React 18, TypeScript
- **Styling**: Tailwind CSS
- **Authentication**: JWT tokens
- **Storage**: Local file system (JSON-based)
- **Real-time**: Polling-based updates

## Getting Started

### Prerequisites

- Node.js 18+ installed
- npm or yarn package manager

### Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd seju
```

2. Install dependencies:
```bash
npm install
```

3. Run the development server:
```bash
npm run dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

### Building for Production

```bash
npm run build
npm start
```

## Deployment

This app is ready for deployment on Vercel:

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Deploy automatically

## Project Structure

```
src/
├── app/                    # Next.js App Router pages
│   ├── api/               # API routes
│   ├── auth/              # Authentication pages
│   ├── chat/              # Chat functionality
│   ├── messages/          # Messages overview
│   ├── post/              # Individual post pages
│   ├── users/             # User discovery
│   └── globals.css        # Global styles
├── components/            # Reusable components
├── hooks/                 # Custom React hooks
└── lib/                   # Utility functions
    └── localStorage.ts    # File-based storage system
```

## Features Overview

### Authentication System
- Secure user registration and login
- JWT token-based authentication
- Password hashing with bcrypt

### Social Features
- Create posts with text and images
- Like and comment on posts
- Share posts with others
- User profiles and discovery

### Messaging System
- Real-time one-on-one chat
- Message notifications
- Conversation management
- Online/offline status tracking

### Online Status
- Real-time user presence
- Heartbeat system for activity tracking
- Visual indicators throughout the app
- 5-minute activity timeout

## API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login

### Posts
- `GET /api/posts` - Retrieve all posts
- `POST /api/posts` - Create new post
- `POST /api/posts/[id]/like` - Toggle post like
- `GET /api/posts/[id]/comments` - Get post comments
- `POST /api/posts/[id]/comments` - Add comment

### Users
- `GET /api/users` - Get all users
- `POST /api/users/heartbeat` - Update user activity

### Chat
- `GET /api/chat/conversations` - Get user conversations
- `GET /api/chat/[userId]` - Get conversation messages
- `POST /api/chat/[userId]` - Send message

### Upload
- `POST /api/upload/image` - Upload image files

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License.

## Support

For support, email your-email@example.com or create an issue in the repository.
