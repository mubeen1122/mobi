# Ogr System App

A professional fleet management application for automated driver attendance tracking and shift management.

## Installation

1. Clone this repository
2. Run `npm install` to install dependencies
3. Configure your database using the `DATABASE_URL` environment variable
4. Run `npm run db:push` to set up the database schema
5. Run `npm run dev` to start the development server

## Features

- Driver attendance tracking with geolocation verification
- Shift scheduling and management
- Automatic absence detection
- Comprehensive admin panel
- Truck assignment and management
- Mobile-responsive design

## Configuration

### Database Setup

This application uses PostgreSQL for data storage. You need to set up a PostgreSQL database and configure the connection using the `DATABASE_URL` environment variable in the format:

```
postgresql://username:password@hostname:port/database_name
```

### Environment Variables

Create a `.env` file in the root directory with the following variables:

```
DATABASE_URL=postgresql://username:password@hostname:port/database_name
SESSION_SECRET=your_random_session_secret
```

## Deployment Requirements

- Node.js 18 or higher
- PostgreSQL 13 or higher
- Internet connection for geolocation services

## Mobile Usage

For proper functionality on mobile devices, the application needs to be served over HTTPS to access geolocation features.