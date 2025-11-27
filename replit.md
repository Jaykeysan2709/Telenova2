# Tale-Nova - Interactive African Storytelling Platform

## Overview
Tale-Nova is an educational storytelling application designed for children ages 4-13 in the African diaspora and across Africa. The platform's tagline is "telling old african stories in a new way". The platform connects young learners with African folklore, languages, and cultural wisdom through interactive stories, AI-powered story generation, language learning modules, educational games, and a cultural map of Africa. It aims to provide a playful, culturally authentic learning experience with a focus on age-appropriate content.

## User Preferences
Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend
The frontend uses React with TypeScript, Vite, Wouter for routing, TanStack Query for data fetching, and Tailwind CSS for styling. It features a custom design system inspired by Duolingo and Khan Academy Kids, utilizing shadcn/ui components with a "New York" style variant, warm color palette, and playful typography (Baloo 2, DM Sans/Inter). State management is handled by TanStack Query for server state, React Hook Form for form state with Zod validation, and React hooks/context for UI state.

### Backend
The backend is built with Express.js on Node.js using TypeScript, providing RESTful API endpoints for stories, user progress, language phrases, proverbs, badges, and game scores. Data is stored in a Neon-hosted PostgreSQL database, accessed via Drizzle ORM for type-safe queries.

### Authentication
Talenova supports dual authentication:
1.  **Local Email/Password:** Self-managed using Passport.js Local Strategy with bcrypt for password hashing and session-based authentication.
2.  **OAuth Social Login:** Integration with Replit's OpenID Connect provider (Google, GitHub, X, Apple, email) using Passport.js.
User accounts can be linked across both methods, and authentication state is managed securely with server-side sessions.

### AI Integration
The platform integrates with OpenAI (via Replit AI Integrations) using GPT-5 for AI-powered story generation. Users can input character, moral, theme, and age group to generate culturally authentic African folktales.

### Data Models
Core entities include:
*   **Story**: Title, content, region, category, age group, moral, cultural context.
*   **UserProgress**: Completed stories, points, badges, streak.
*   **LanguagePhrase**: Phrase, translation, pronunciation, category.
*   **Proverb**: Text, meaning, culture, category.
*   **Badge**: Achievement tracking.
*   **GameScore**: User game performance.
These models are defined with Drizzle ORM schemas and validated using Zod for type safety.

### Application Features
Key features include:
*   **Story Library**: Categorized collection of African folklore with filtering and audio narration.
*   **AI Story Builder**: User-driven AI story generation.
*   **Language Learning**: Interactive flashcards, daily challenges, and pronunciation guides for African languages.
*   **Educational Games**: Mini-games like "Guess the Animal," "Match the Proverb," and "Story Origin."
*   **Cultural Map**: Interactive map exploring African countries, stories, and languages by region.
*   **Progress Tracking**: User progress, points, badges, and learning streaks are tracked and persisted.

## External Dependencies

*   **Frontend**: React, Vite, Wouter, TanStack Query, Tailwind CSS, shadcn/ui, Radix UI, Lucide React, React Hook Form, Zod.
*   **Backend**: Express.js, Node.js, TypeScript.
*   **Database**: PostgreSQL (Neon), Drizzle ORM, @neondatabase/serverless, connect-pg-simple.
*   **Authentication**: Passport.js, passport-local, bcrypt, express-session.
*   **AI Services**: OpenAI SDK (via Replit AI Integrations).
*   **Utilities**: class-variance-authority (cva), clsx, tailwind-merge, date-fns, nanoid, cmdk, embla-carousel-react.
*   **Development Tools**: @replit/vite-plugin-runtime-error-modal, @replit/vite-plugin-cartographer, @replit/vite-plugin-dev-banner, tsx, esbuild.