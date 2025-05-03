# FitFeed - Fitness & Nutrition Social App

FitFeed is a TikTok-inspired fitness and nutrition tracking app that combines short-form video content with AI-powered nutrition tracking and health features.

## Features

- **Social Feed**: View and share workout videos in a vertical scrolling feed similar to TikTok
- **Meal Logging**: Take photos of meals, get AI-powered nutritional analysis
- **AI Nutritionist**: Chat with an AI assistant for personalized nutrition advice
- **Progress Tracking**: Monitor your fitness journey with detailed statistics and visualizations
- **User Profiles**: Share your fitness journey and connect with like-minded individuals

## How to Deploy on GitHub

### 1. Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in to your account
2. Click on the "+" button in the upper right corner and select "New repository"
3. Name your repository (e.g., "fitfeed-app")
4. Choose the visibility (public or private)
5. Click "Create repository"

### 2. Push Your Code to GitHub

From your terminal/command prompt:

```bash
# Initialize Git in your project directory (if not already done)
git init

# Add all files to staging
git add .

# Commit your changes
git commit -m "Initial commit"

# Add the GitHub repository as a remote
git remote add origin https://github.com/your-username/fitfeed-app.git

# Push your code to GitHub
git push -u origin main
```

### 3. Deploy with GitHub Pages (Static Frontend Only)

For simple static frontend only:

1. In your GitHub repository, go to Settings > Pages
2. Under "Source", select "Deploy from a branch"
3. Choose your main branch and the folder containing your frontend code (usually `/client` or `/build`)
4. Click "Save"

Your site will be published at `https://your-username.github.io/fitfeed-app/`

### 4. Deploy Full Stack App with Render, Railway, or Vercel

For full-stack deployment with database:

#### Using Render:

1. Create an account on [Render](https://render.com/)
2. Connect your GitHub repository
3. Create a new Web Service for your backend
4. Configure environment variables (DATABASE_URL, OPENAI_API_KEY, etc.)
5. Deploy the service

#### Using Railway:

1. Create an account on [Railway](https://railway.app/)
2. Connect your GitHub repository
3. Create a new project
4. Add a PostgreSQL database service
5. Configure environment variables
6. Deploy your app

#### Using Vercel:

1. Create an account on [Vercel](https://vercel.com/)
2. Connect your GitHub repository
3. Configure your project settings
4. Add environment variables
5. Deploy your app

## Environment Variables

Make sure to set these environment variables in your deployment platform:

- `DATABASE_URL`: PostgreSQL database connection string
- `OPENAI_API_KEY`: Your OpenAI API key for AI features
- `SESSION_SECRET`: A random string for securing sessions

## Local Development

```bash
# Install dependencies
npm install

# Start the development server
npm run dev
```

The app will be available at http://localhost:5000

## License

This project is licensed under the MIT License - see the LICENSE file for details.