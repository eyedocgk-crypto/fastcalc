# FastTracker - Intermittent Fasting Calculator

## Overview

FastTracker is a modern single-page web application that helps users calculate and track their intermittent fasting schedules. The app provides personalized meal timing calculations for popular fasting protocols (16:8, 18:6, and 20:4), along with helpful tips and real-time countdown features. Built with React frontend and Express backend, it features Google AdSense integration with authentic banner styling throughout the page for monetization.

## Recent Changes (August 2025)

- ✅ **Complete Calculator Implementation**: Built comprehensive fasting calculator with age, sex, and protocol inputs
- ✅ **Real-time Countdown**: Added live countdown timer showing remaining fasting time
- ✅ **Personalized Tips**: Implemented age and sex-specific fasting recommendations
- ✅ **Google AdSense Integration**: Added multiple authentic-styled banner placements (header, rectangle, square, horizontal)
- ✅ **Timezone Fix**: Resolved 1-hour timing offset by properly handling datetime-local inputs and timezone calculations
- ✅ **BMI Calculator Addition**: Added comprehensive BMI calculator with metric/imperial unit support, BMI categories, and health recommendations
- ✅ **Enhanced SEO**: Updated meta tags to include BMI functionality for better search visibility
- ✅ **Modern UI**: Clean, responsive design with proper form validation and smooth scrolling

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript for type safety and modern React features
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: TanStack Query (React Query) for server state management and caching
- **Form Handling**: React Hook Form with Zod validation for type-safe form validation
- **UI Components**: Radix UI primitives with shadcn/ui for accessible, customizable components
- **Styling**: Tailwind CSS with CSS variables for theming and responsive design
- **Build Tool**: Vite for fast development and optimized production builds

### Backend Architecture
- **Runtime**: Node.js with TypeScript for type safety across the stack
- **Framework**: Express.js for RESTful API endpoints
- **Database Layer**: Drizzle ORM with PostgreSQL for type-safe database operations
- **Storage**: Abstracted storage interface with in-memory implementation for development
- **Build System**: ESBuild for fast server-side compilation

### Data Storage Solutions
- **Database**: PostgreSQL with Neon serverless for production scalability
- **ORM**: Drizzle ORM for type-safe database queries and migrations
- **Schema Management**: Centralized schema definitions in `shared/schema.ts` for consistency
- **Migrations**: Drizzle Kit for database migration management

### Authentication and Authorization
- **Session Management**: Connect-pg-simple for PostgreSQL-backed session storage
- **User Model**: Basic user schema with username/password authentication ready for implementation
- **Security**: Prepared for secure session handling and user authentication flows

### External Dependencies
- **Database**: Neon serverless PostgreSQL for cloud-native data persistence
- **UI Framework**: Radix UI for accessible component primitives
- **Validation**: Zod for runtime type checking and form validation
- **Date Handling**: date-fns for reliable date manipulation and formatting
- **Development**: Replit-specific tooling for seamless cloud development experience

The application follows a monorepo structure with clear separation between client, server, and shared code, enabling type safety across the entire stack while maintaining modularity and scalability.