# Hela Link Loan Application

A Full-Stack loan application system with user submission, admin dashboard, and SQLite database.

## Features

- User loan submission system
- Admin dashboard for loan management
- SQLite database integration
- Real-time application tracking
- **Vercel Web Analytics** for tracking page views and user interactions

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm, yarn, pnpm, or bun

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Deon99894/hela-link-loan-app.git
   cd hela-link-loan-app
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

4. Open your browser and navigate to `http://localhost:3000`

## Vercel Web Analytics

This project is configured with Vercel Web Analytics to track page views and user interactions.

### How It Works

The analytics are automatically loaded when you deploy to Vercel. The implementation uses the HTML/Vanilla JS approach:

1. The analytics script is included in `index.html`
2. The `window.va` function is initialized to queue events
3. Vercel's analytics script (`/_vercel/insights/script.js`) is loaded asynchronously

### Local Development

Analytics will not track events in local development. They only work when deployed to Vercel.

### Deployment

To deploy to Vercel:

1. Install Vercel CLI:
   ```bash
   npm i -g vercel
   ```

2. Deploy:
   ```bash
   vercel deploy
   ```

3. Enable Web Analytics in your Vercel project dashboard:
   - Go to your project settings
   - Navigate to Analytics
   - Click "Enable"

### Verification

After deployment, you can verify that analytics are working by:
1. Opening your deployed site
2. Opening browser DevTools (Network tab)
3. Looking for requests to `/_vercel/insights/view`

## Scripts

- `npm start` - Start the server
- `npm run dev` - Start in development mode
- `npm test` - Run tests (to be implemented)

## Project Structure

```
hela-link-loan-app/
├── index.html          # Main HTML file with Vercel Analytics
├── app.js             # Application JavaScript
├── server.js          # Node.js HTTP server
├── package.json       # Project dependencies
├── .gitignore         # Git ignore rules
└── README.md          # This file
```

## Technologies Used

- **Backend**: Node.js (vanilla HTTP server)
- **Frontend**: HTML, CSS, JavaScript
- **Database**: SQLite (to be implemented)
- **Analytics**: Vercel Web Analytics
- **Deployment**: Vercel

## License

ISC
