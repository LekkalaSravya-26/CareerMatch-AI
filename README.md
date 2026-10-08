# CareerMatch AI

AI-powered career discovery platform that matches you with your ideal career path based on a personality, skills, and interests assessment.

## Features

- **Intelligent Assessment** — 12-question quiz covering 8 career dimensions
- **AI Matching Engine** — Scores compatibility across 16 career paths
- **Detailed Career Profiles** — Salary, growth outlook, education, day-to-day, pros & cons
- **Save Results** — Store your assessment results with Supabase
- **Responsive Design** — Works beautifully on mobile, tablet, and desktop

## Tech Stack

- React 18 + TypeScript
- Vite 5
- Tailwind CSS 3
- Supabase (database)
- Lucide React (icons)

## Getting Started

### Prerequisites

- Node.js 18+ and npm
- A Supabase project (for data persistence)

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/career-match-ai.git
cd career-match-ai

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your Supabase URL and anon key

# Run development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

### Environment Variables

Create a `.env` file in the project root:

```
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

### Database Setup

The app uses a single `assessment_results` table. The migration is applied automatically via Supabase MCP tools. If setting up manually, run the SQL from the migration in your Supabase SQL editor.

## Project Structure

```
src/
  components/     # UI components (Navbar, Footer, Landing, Quiz, Results, etc.)
  data/           # Career definitions and quiz questions
  lib/            # Supabase client and data access functions
  types/          # TypeScript type definitions
  utils/          # Career matching algorithm
  App.tsx         # Main app with view routing
  main.tsx        # React entry point
  index.css       # Global styles + Tailwind
```

## Running in VS Code

1. Open the project folder in VS Code
2. Install the recommended extensions (ESLint, Prettier, Tailwind CSS IntelliSense)
3. Open a terminal (`Ctrl + \``) and run `npm install`
4. Run `npm run dev` to start the development server
5. Open the URL shown in the terminal (typically `http://localhost:5173`)

## Transferring to GitHub

1. Create a new repository on GitHub
2. In the project folder, run:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: CareerMatch AI"
   git branch -M main
   git remote add origin https://github.com/your-username/career-match-ai.git
   git push -u origin main
   ```

## License

MIT
