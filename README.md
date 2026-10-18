# MathLevel AI

A simple, responsive mathematics learning website with three difficulty levels and an AI-style practice experience.

## Live preview

Open `index.html` directly in a browser. The project is fully self-contained and does not require installation, a server, a database, or API keys.

## Features

- Foundation, Standard, and Advanced levels
- Generated practice questions
- Answer checking
- Helpful hints
- Step-by-step explanations
- Adaptive guidance based on selected level
- Solved-question and correct-answer dashboard
- Progress bar
- Responsive mobile and desktop layout
- Purple and blue visual design with smooth interactions

## Run locally

1. Download or unzip the project.
2. Open `index.html` in any modern browser.
3. Select a level and start practicing.

No build step is required.

## Deploy to GitHub Pages

1. Create a new public GitHub repository, for example `mathlevel-ai`.
2. Upload `index.html`, `README.md`, and `REPORT.md`.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/root` folder, then save.
6. GitHub will provide the public website URL.

## Deploy to Netlify

1. Create a free Netlify account.
2. Choose **Add new site → Deploy manually**.
3. Drag the project folder into the upload area.
4. Netlify will provide a public URL immediately.

## Deploy to Vercel

1. Create a free Vercel account.
2. Import the GitHub repository, or use the Vercel dashboard upload flow.
3. Keep the default settings because this is a static HTML project.
4. Deploy and copy the generated public URL.

## AI demo note

The current version intentionally works without external API keys. Its adaptive experience is implemented with local JavaScript rules and curated explanations, so it is safe to demo offline. The interface is ready for a real AI service later, but no external service is required for the working demo.
