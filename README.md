# BuyerIQ: Real Estate Analytics Platform

BuyerIQ (formerly FlipIQ) is a sophisticated real estate analytics platform that leverages intelligent data processing to transform complex market insights into actionable intelligence for real estate professionals.

## Overview

BuyerIQ is designed to provide comprehensive analytics for different types of real estate professionals:

- **Investors**: Track investment activity, analyze purchase-to-resale ratios, and identify profitable investment patterns
- **Agents**: Analyze transaction history with investors, double-end transactions, and relationship patterns
- **Offices**: Review brokerage-level metrics, buyer representation trends, and market positioning
- **Lenders**: Monitor loan activity, average loan amounts, and relationships with real estate investors

The platform integrates with an external property database containing over 35,000 records and provides advanced filtering capabilities for precise data retrieval.

## Key Features

### Advanced Filtering

- Location-based filtering (County → City → ZIP Code waterfall)
- Real-time data updates with cascading selections
- Additional entity-specific filters (transaction volume, price ranges, etc.)
- Radius-based searches around specified addresses

### Data Visualization

- Transaction history charts
- Investment performance metrics
- Relationship mapping between entities
- Market trend analysis

### Communication & Outreach Module

The Communication & Outreach Module is integrated into the Investor and Agent modules with multiple components:

- **DialPad**: Make VoIP calls and send text messages directly from the platform
- **Text Bot**: Schedule and run SMS campaigns with personalized messages
- **Email Bot**: Create and manage targeted email campaigns
- **AI Connect**: Engage in conversational interactions using AI assistance
- **Direct-to-Voicemail**: Send pre-recorded messages directly to voicemail

## Technical Stack

- **Frontend**: React with TypeScript, Tailwind CSS for responsive design
- **State Management**: React Query for data fetching and caching
- **UI Components**: ShadCN component library with custom theming
- **Backend**: Express.js API server
- **Database**: PostgreSQL with Drizzle ORM for schema management
- **External Database Connection**: Secure connection to property database via Neon Serverless PostgreSQL

## Getting Started

### Prerequisites

- Node.js (v18+)
- PostgreSQL database

### Installation

1. Clone the repository
2. Install dependencies: `npm install` 
3. Set up environment variables (see `.env.example`)
4. Run the development server: `npm run dev`

### Environment Variables

The application requires the following environment variables:

- `DATABASE_URL`: PostgreSQL connection string for the main application database
- `EXTERNAL_DATABASE_URL`: Connection string for the external property database
- `SESSION_SECRET`: Secret key for session management

## Data Architecture

The application uses a dual-database approach:

1. **Main Database**: Stores application data including users, saved searches, communication records, and entity relationships
2. **External Database**: Contains property records (35,636 properties) with detailed information about real estate transactions

## Usage

1. Navigate to the dashboard
2. Select the tab for the entity type you want to analyze (Investors, Agents, Offices, Lenders)
3. Apply filters to narrow down results
4. View detailed analytics and export data as needed
5. Use the Communication module to engage with selected entities

## License

This project is proprietary software. All rights reserved.

## Support

For support or feature requests, please contact support@buyeriq.com
