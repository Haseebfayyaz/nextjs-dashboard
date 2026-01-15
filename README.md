# Next.js Dashboard Application

A modern, full-stack dashboard application built with Next.js App Router, featuring invoice management, customer tracking, and revenue analytics.

## 🚀 Features

- **Dashboard Overview**: Real-time revenue charts and latest invoice tracking
- **Invoice Management**: Create, edit, and manage invoices with status tracking
- **Customer Management**: View and manage customer information
- **Authentication**: Secure login system with NextAuth
- **Responsive Design**: Mobile-first design with Tailwind CSS
- **Type Safety**: Full TypeScript support
- **Database Integration**: PostgreSQL database with optimized queries

## 🛠️ Tech Stack

- **Framework**: [Next.js](https://nextjs.org/) (App Router)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **Database**: [PostgreSQL](https://www.postgresql.org/)
- **Authentication**: [NextAuth.js](https://next-auth.js.org/)
- **Icons**: [Heroicons](https://heroicons.com/)
- **Validation**: [Zod](https://zod.dev/)
- **Package Manager**: [pnpm](https://pnpm.io/)

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v18 or higher)
- [pnpm](https://pnpm.io/installation) (or npm/yarn)
- [PostgreSQL](https://www.postgresql.org/download/) database

## 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd nextjs-dashboard
   ```

2. **Install dependencies**
   ```bash
   pnpm install
   ```

3. **Set up environment variables**
   
   Create a `.env.local` file in the root directory:
   ```env
   POSTGRES_URL=your_postgres_connection_string
   AUTH_SECRET=your_auth_secret_key
   ```

4. **Set up the database**
   
   Run the seed script to populate the database with sample data:
   ```bash
   pnpm run seed
   ```
   
   Or visit `/seed` route in your browser after starting the development server.

## 🚀 Getting Started

1. **Start the development server**
   ```bash
   pnpm dev
   ```

2. **Open your browser**
   
   Navigate to [http://localhost:3000](http://localhost:3000)

3. **Login**
   
   Use the login page to access the dashboard. Default credentials can be found in the seed data.

## 📜 Available Scripts

- `pnpm dev` - Start the development server with Turbopack
- `pnpm build` - Build the application for production
- `pnpm start` - Start the production server

## 📁 Project Structure

```
nextjs-dashboard/
├── app/
│   ├── dashboard/          # Dashboard pages
│   │   ├── customers/      # Customer management
│   │   ├── invoices/       # Invoice management
│   │   ├── layout.tsx      # Dashboard layout
│   │   └── page.tsx        # Dashboard home
│   ├── lib/                # Utility functions and data
│   │   ├── data.ts         # Database queries
│   │   ├── definitions.ts  # TypeScript type definitions
│   │   ├── utils.ts        # Helper functions
│   │   └── placeholder-data.ts
│   ├── ui/                 # Reusable UI components
│   │   ├── dashboard/      # Dashboard-specific components
│   │   ├── invoices/       # Invoice-related components
│   │   └── customers/      # Customer-related components
│   ├── layout.tsx          # Root layout
│   └── page.tsx            # Home page
├── public/                 # Static assets
└── package.json
```

## 🗄️ Database Schema

The application uses the following main entities:

- **Users**: Authentication and user management
- **Customers**: Customer information and profiles
- **Invoices**: Invoice records with status tracking
- **Revenue**: Monthly revenue data for analytics

## 🎓 Learning Resources

This project is part of the [Next.js Learn Course](https://nextjs.org/learn). For more information and detailed tutorials, visit the [course curriculum](https://nextjs.org/learn) on the Next.js website.

## 📝 Notes

- This is a learning project based on the Next.js App Router Course
- The database connection uses SSL by default
- Some artificial delays are included in the code for demonstration purposes (not recommended for production)

## 🤝 Contributing

This is a learning project. Feel free to fork and experiment with your own modifications!

## 📄 License

This project is created for educational purposes as part of the Next.js Learn Course.
