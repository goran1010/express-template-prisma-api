# Express Prisma Backend Template

A template for Express.js backend applications with Prisma ORM and session-based authentication.

## Features

- Express.js
- Prisma ORM with PostgreSQL
- Session-based authentication using Passport.js
- CORS enabled for frontend integration
- ESLint and Prettier configuration
- Jest testing setup
- Environment configuration

## Prerequisites

- Node.js (v18 or higher)
- PostgreSQL database server
- npm or yarn

## Database Requirements

Before installation, make sure to:

1. Create a PostgreSQL database for development
2. Create a separate PostgreSQL database for testing
3. Note down your database credentials for the `.env` file

## Installation

```bash
# Clone the repository
git clone https://github.com/goran1010/template-express-prisma-backend-session.git

# Navigate to project directory
cd template-express-prisma-backend-session

# Install dependencies
npm install

# Setup environment variables
cp .env.example .env
# Edit .env with your database credentials and secret

# Initialize database and run migrations
npx prisma migrate dev
```

## Usage

```bash
# Start development server with hot reload
npm run dev

# Start production server
npm run start

# Run tests
npm run test
```

## Environment Variables

- `DATABASE_URL`: PostgreSQL URL for development database
- `TEST_DATABASE_URL`: PostgreSQL URL for test database
- `SECRET`: Session secret key
- `PORT`: Server port (defaults to 3000)

## License

MIT
