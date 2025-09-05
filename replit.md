# replit.md

## Overview

CyberGuard is a network security monitoring dashboard built as a full-stack web application. The system provides cybersecurity professionals with tools to monitor network devices, track security vulnerabilities, manage user access, and visualize security metrics through an intuitive interface.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React with TypeScript using Vite as the build tool
- **Styling**: Tailwind CSS with shadcn/ui component library for consistent design
- **State Management**: TanStack Query for server state management and data fetching
- **Routing**: Wouter for client-side routing
- **Charts**: Recharts for data visualization
- **Component System**: Radix UI primitives with custom styling through shadcn/ui

### Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **Development**: tsx for TypeScript execution in development
- **Production**: esbuild for backend bundling

### Data Storage Solutions
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **Schema Management**: Drizzle Kit for migrations and schema management
- **Development Storage**: In-memory storage implementation for development/testing
- **Session Storage**: PostgreSQL-based session storage using connect-pg-simple

### Authentication and Authorization
- **Role-Based Access**: Three-tier system (admin, analyst, viewer)
- **User Management**: CRUD operations for user accounts with role assignment
- **Session Management**: Express sessions with PostgreSQL storage

### API Architecture
- **Pattern**: RESTful API design
- **Routes**: Organized by feature (users, dashboard, devices)
- **Validation**: Zod schemas for request/response validation
- **Error Handling**: Centralized error middleware with structured responses

### UI/UX Design Decisions
- **Theme**: Dark mode by default with CSS custom properties for theming
- **Responsive Design**: Mobile-first approach with Tailwind breakpoints
- **Component Library**: shadcn/ui for consistent, accessible components
- **Icon System**: Lucide React for consistent iconography

## External Dependencies

### Database Services
- **Neon Database**: Serverless PostgreSQL database hosting
- **Connection**: @neondatabase/serverless for database connectivity

### UI Component Libraries
- **Radix UI**: Comprehensive set of accessible, unstyled UI primitives
- **shadcn/ui**: Pre-styled components built on Radix UI
- **Tailwind CSS**: Utility-first CSS framework for styling

### Development Tools
- **Drizzle**: Type-safe ORM and schema management
- **Vite**: Fast build tool and development server
- **TypeScript**: Type safety across the full stack
- **Zod**: Runtime type validation for API endpoints

### Third-Party Integrations
- **Replit**: Development environment integration with runtime error handling
- **Google Fonts**: Web fonts (DM Sans, Architects Daughter, Fira Code, Geist Mono)
- **Chart Libraries**: Recharts for security metrics visualization

### Key Features
- **Device Monitoring**: Track network devices with risk scoring
- **CVE Tracking**: Monitor security vulnerabilities with severity levels
- **Port Scanning**: Detect and analyze open ports across the network
- **User Management**: Role-based access control system
- **Dashboard Analytics**: Visual representation of security metrics