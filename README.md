# Discover Coffee Stores

A web application that helps users discover coffee stores in their vicinity and in Toronto. Built with Next.js and React, this application provides an interactive way to find, view, and rate coffee shops.

## Features

- **Discover Nearby Coffee Stores**: Uses geolocation to find coffee shops near the user's location
- **Browse Toronto Coffee Stores**: View a curated list of coffee stores in Toronto
- **Detailed Store Information**: View detailed information about each coffee store including address, neighborhood, and ratings
- **Upvote Stores**: Users can upvote their favorite coffee stores
- **Responsive Design**: Optimized for both desktop and mobile devices

## Tech Stack

### Frontend
- **Next.js**: React framework for server-side rendering and static site generation
- **React**: JavaScript library for building user interfaces
- **CSS Modules**: For component-scoped styling

### Backend & API
- **Next.js API Routes**: Serverless functions for backend operations
- **Foursquare API**: For fetching coffee store data
- **Unsplash API**: For fetching high-quality coffee store images
- **Airtable**: Database for storing user interactions and coffee store data

### Data Fetching & State Management
- **SWR**: React Hooks library for data fetching and caching
- **Context API**: For global state management

### Other Libraries
- **classnames**: Utility for conditionally joining classNames
- **unsplash-js**: JavaScript wrapper for the Unsplash API

## Getting Started

### Prerequisites
- Node.js 14.x or later
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/discover-coffee-stores.git
cd discover-coffee-stores
```

2. Install dependencies
```bash
npm install
# or
yarn install
```

3. Create a `.env.local` file in the root directory with the following environment variables:
```
NEXT_PUBLIC_FOURSQUARE_API_KEY=your_foursquare_api_key
NEXT_PUBLIC_UNSPLASH_ACCESS_KEY=your_unsplash_access_key
AIRTABLE_API_KEY=your_airtable_api_key
AIRTABLE_BASE_ID=your_airtable_base_id
```

4. Start the development server
```bash
npm run dev
# or
yarn dev
```

5. Open [http://localhost:3000](http://localhost:3000) with your browser to see the application.

## Project Structure

- **pages/**: Contains all the pages and API routes
  - **api/**: API routes for coffee store operations
  - **coffee-store/**: Dynamic routes for individual coffee store pages
- **components/**: Reusable React components
- **styles/**: CSS modules for styling
- **data/**: API integration with Foursquare and Unsplash
- **hooks/**: Custom React hooks for location and data fetching
- **lib/**: Utility functions and Airtable API integration
- **context/**: React Context for global state management
- **public/**: Static assets like images

## Deployment

The application can be easily deployed on [Vercel](https://vercel.com), the platform from the creators of Next.js.

```bash
npm run build
# or
yarn build
```

## License

This project is open source and available under the [MIT License](LICENSE).
