# React News App

A modern, responsive news aggregation application built with React that fetches and displays news articles from the GNews API. Users can browse news across multiple categories and discover the latest stories from around the world.

## Features

- 📰 **Multi-Category News**: Browse news across 8 different categories:
  - General
  - Business
  - Entertainment
  - Health
  - Science
  - Sports
  - Technology

- 🔄 **Infinite Scroll**: Seamlessly load more articles as you scroll down the page
- 📊 **Loading Progress Bar**: Visual feedback while fetching news data
- 🎨 **Responsive Design**: Built with Bootstrap for excellent mobile and desktop experience
- 🧭 **Navigation Bar**: Easy navigation between different news categories
- ⚡ **React 18**: Modern React with hooks (useState, useEffect, useCallback)

## Technology Stack

- **Frontend Framework**: React 18.3.1
- **UI Framework**: Bootstrap 5.3.3 with React-Bootstrap 2.10.2
- **Routing**: React Router DOM 6.23.1
- **Infinite Scroll**: react-infinite-scroll-component 6.1.0
- **Loading Bar**: react-top-loading-bar 2.3.1
- **News API**: GNews API

## Project Structure

```
ReactNews/
├── public/
│   ├── index.html
│   ├── manifest.json
│   └── robots.txt
├── src/
│   ├── components/
│   │   ├── Navigationbar.js      # Navigation menu component
│   │   ├── News.js               # Main news fetching and display component
│   │   └── Newsitem.js           # Individual news article card component
│   ├── App.js                    # Main application component with routing
│   ├── App.css                   # Application styles
│   ├── index.js                  # React entry point
│   ├── index.css                 # Global styles
│   ├── reportWebVitals.js        # Performance monitoring
│   ├── setupTests.js             # Test configuration
│   └── sampleOutput.json         # Sample API response data
├── package.json                  # Project dependencies and scripts
├── vercel.json                   # Vercel deployment configuration
└── README.md                     # This file
```

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn package manager

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd ReactNews
```

2. Install dependencies:
```bash
npm install
```

3. Obtain a GNews API key from [https://gnews.io](https://gnews.io)

4. Add your API key to `src/App.js`:
```javascript
const apiKey = "your_api_key_here";
```

### Running the Application

Start the development server:
```bash
npm start
```

The application will open at [http://localhost:3000](http://localhost:3000) in your browser.

## Available Scripts

- `npm start` - Runs the app in development mode
- `npm build` - Builds the app for production
- `npm test` - Launches the test runner
- `npm eject` - Ejects from Create React App (irreversible)

## API Configuration

The application uses the GNews API with the following configuration:
- **Language**: English
- **Country**: India (changeable in `App.js`)
- **Page Size**: 6 articles per page (configurable)
- **API Proxy**: Configured via `package.json` proxy setting

## Component Overview

### App.js
Main application component that:
- Manages routing for different news categories
- Handles loading progress state
- Sets up the LoadingBar component
- Passes API configuration to News component

### News.js
Core component that:
- Fetches news articles from the GNews API
- Implements infinite scroll functionality
- Manages article state and pagination
- Displays loading spinner during data fetch
- Handles errors gracefully

### Newsitem.js
Presentation component that displays individual news articles with:
- Article image
- Title
- Description
- Link to full article

### Navigationbar.js
Navigation component providing links to all news categories

## Key Features Implementation

### Infinite Scroll
Utilizes `react-infinite-scroll-component` to automatically load more articles when the user scrolls near the bottom of the page.

### Loading Progress
Displays a progress bar at the top of the page using `react-top-loading-bar` to provide visual feedback during API calls.

### Error Handling
The News component includes error handling for:
- Network failures
- Invalid API responses
- Empty result sets

### Responsive Layout
Uses Bootstrap Grid system for responsive design that adapts to all screen sizes.

## Future Enhancements

- Search functionality
- Article bookmarking/favorites
- Dark mode toggle
- Category filtering options
- Read time estimation
- Social sharing features
- Local storage for saved articles

## Environment Variables

Consider moving sensitive data like API keys to environment variables:

```bash
REACT_APP_API_KEY=your_api_key_here
REACT_APP_COUNTRY=in
REACT_APP_PAGE_SIZE=6
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Deployment

The project includes `vercel.json` configuration for easy deployment to Vercel:

```bash
npm run build
# Deploy using Vercel CLI or connect your GitHub repo
```

## License

This project is private and not open for public use.

## Support

For issues, questions, or suggestions, please create an issue in the repository.

---

**Built with ❤️ using React**

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
>>>>>>> 5566971 (Initial commit)
>>>>>>> c9adf26 (first commit)
