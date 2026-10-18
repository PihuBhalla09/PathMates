# PathMates

PathMates is a platform that helps students connect with alumni, explore career opportunities, save professional connections, and request mentorship sessions.

## Features

- **Alumni Directory:** Discover alumni and explore their professional backgrounds.
- **Search and Filters:** Find relevant alumni and opportunities.
- **Career Opportunities:** Browse internships, jobs, and other opportunities.
- **Saved Connections:** Save alumni profiles for future reference.
- **Mentorship Requests:** Request mentorship sessions with alumni.
- **Authentication:** Sign in using email-based OTP authentication.
- **Responsive Design:** Access the platform across desktop and mobile devices.

## Tech Stack

- **Frontend:** React, Vite
- **Styling:** CSS
- **Icons:** Lucide React
- **Backend and Database:** Supabase
- **Authentication:** Supabase Auth

## Getting Started

### Prerequisites

Make sure you have the following installed:

- Node.js
- npm
- A Supabase account



4. Create a `.env.local` file in the root directory.

5. Add your Supabase project credentials:

   ```env
   VITE_SUPABASE_URL=your_supabase_project_url
   VITE_SUPABASE_ANON_KEY=your_supabase_publishable_or_anon_key
   ```

6. Start the development server:

   ```bash
   npm run dev
   ```

7. Open the local URL displayed in your terminal.

## Supabase Setup

PathMates uses Supabase for database operations and authentication.

The application expects the following tables:

- `alumni`
- `opportunities`
- `saved_connections`
- `session_requests`

Make sure the database tables, columns, authentication settings, and Row Level Security policies match the application's requirements.

## Environment Variables

| Variable | Description |
|---|---|
| `VITE_SUPABASE_URL` | Your Supabase project URL |
| `VITE_SUPABASE_ANON_KEY` | Your Supabase publishable key or legacy anon key |

Never expose your Supabase service role key in frontend code or commit secret credentials to GitHub.

## Project Structure

```text
PathMates/
├── public/
├── src/
│   ├── lib/
│   │   └── supabaseClient.js
│   ├── App.jsx
│   ├── App.css
│   └── index.css
├── .env.local
├── .gitignore
├── index.html
├── package.json
└── README.md
```

The exact structure may vary depending on your project setup.

## Security

- Keep `.env.local` out of version control.
- Never commit private API keys or service role keys.
- Configure appropriate Row Level Security policies in Supabase.
- Restrict access to user-specific data.

## Contributing

Contributions and suggestions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Open a pull request.

## License

No license has been specified yet. Add a license before distributing the project for reuse.
