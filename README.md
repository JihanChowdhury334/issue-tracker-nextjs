# Issue Tracker - Next.js

A full-stack issue tracking application built with Next.js 15, featuring authentication, database integration, and modern React patterns.

## 🚀 Features

- **User Authentication** - Sign up, sign in, and session management with NextAuth.js
- **Issue Management** - Create, view, and manage issues with full CRUD operations
- **Database Integration** - PostgreSQL with Drizzle ORM for type-safe database operations
- **Server Components** - Modern Next.js App Router with server-side rendering
- **Responsive Design** - Clean UI built with Tailwind CSS
- **Type Safety** - Full TypeScript implementation throughout the application

## 🛠️ Tech Stack

- **Framework**: Next.js 15 with App Router
- **Language**: TypeScript
- **Authentication**: NextAuth.js v4
- **Database**: PostgreSQL with Drizzle ORM
- **Styling**: Tailwind CSS
- **Password Hashing**: bcrypt
- **Deployment Ready**: Vercel-optimized

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/JihanChowdhury334/issue-tracker-nextjs.git
   cd issue-tracker-nextjs
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env.local` file in the root directory:
   ```env
   # Database
   DATABASE_URL="your-postgresql-connection-string"

   # NextAuth
   NEXTAUTH_URL="http://localhost:3000"
   NEXTAUTH_SECRET="your-secret-key"
   ```

4. **Set up the database**
   ```bash
   npm run db:generate
   npm run db:migrate
   ```

5. **Start the development server**
   ```bash
   npm run dev
   ```

Visit `http://localhost:3000` to see the application running.

## 🏗️ Project Structure

```
src/
├── app/
│   ├── api/
│   │   ├── auth/[...nextauth]/    # NextAuth configuration
│   │   └── signup/                # User registration endpoint
│   ├── issues/
│   │   ├── new/                   # Create new issue page
│   │   └── page.tsx               # Issues dashboard
│   ├── signin/                    # Sign in page
│   ├── signup/                    # Sign up page
│   └── layout.tsx                 # Root layout with navigation
├── components/
│   ├── Navbar.tsx                 # Navigation component
│   └── Providers.tsx              # Client-side providers wrapper
└── db/
    ├── index.ts                   # Database connection
    └── schema.ts                  # Database schema definitions
```

## 🔑 Key Features Explained

### Authentication System
- Secure user registration and login
- Password hashing with bcrypt
- JWT-based sessions with NextAuth.js
- Protected routes and authentication state management

### Database Schema
- **Users Table**: Stores user accounts and credentials
- **Issues Table**: Manages issue data with foreign key relationships
- **Type-safe Operations**: Drizzle ORM ensures compile-time type checking

### Modern React Patterns
- **Server Components**: Database queries and initial rendering on the server
- **Client Components**: Interactive elements with proper state management
- **Server Actions**: Form handling with server-side processing

## 🚦 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run db:generate` - Generate database migrations
- `npm run db:migrate` - Run database migrations
- `npm run db:studio` - Open Drizzle Studio for database management

## 📋 Usage

1. **Sign Up**: Create a new account with email and password
2. **Sign In**: Log in to access the issue tracker
3. **View Issues**: Browse all issues on the dashboard
4. **Create Issues**: Add new issues with title, description, and status
5. **Navigation**: Use the top navigation bar to move between pages

## 🔮 Roadmap

- [ ] Individual issue detail pages with edit/delete functionality
- [ ] Advanced filtering and search capabilities
- [ ] Issue assignment and priority levels
- [ ] Real-time updates and notifications
- [ ] Enhanced UI components and animations
- [ ] Mobile-responsive improvements

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes and commit: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature-name`
5. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

Built with ❤️ using Next.js 15 and modern web technologies.
