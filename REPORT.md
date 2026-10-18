# MathLevel AI — Brief Report

## Project purpose

MathLevel AI is a responsive educational website that helps students practice algebra at three difficulty levels: Foundation, Standard, and Advanced. The goal is to make mathematics feel approachable by combining short questions, instant feedback, hints, and step-by-step explanations.

## AI prompts used

The project was designed around three prompt patterns that can be connected to a real AI model later:

1. **Question generation prompt**

   “Create one algebra equation for a student at the selected level. Return the equation, the numerical answer, one short hint that does not reveal the answer, and a clear step-by-step solution. Use simple English and avoid unnecessary notation.”

2. **Hint prompt**

   “Give the next helpful algebra step for this equation. Do not give the final answer. Match the explanation to the student’s difficulty level and use simple English.”

3. **Explanation prompt**

   “Explain this solution step by step for a student at the selected level. Foundation should use very simple language, Standard should name the algebra operation at each step, and Advanced should show expansion, collecting like terms, and checking the result.”

The current website is deliberately labeled as an **AI demo**. It does not call an external AI API or require an API key. Instead, it uses a curated local question bank and deterministic JavaScript logic so the demo remains reliable, portable, and easy to deploy.

## How differentiation is achieved

- **Foundation:** one-step equations such as `x + 5 = 12`; hints use direct actions such as “subtract 5 from both sides.”
- **Standard:** two-step equations such as `3(x − 2) = 15`; explanations separate the operations into an ordered process.
- **Advanced:** multi-step equations such as `5(x + 3) + 7 = 2x + 49`; explanations show expansion, moving terms, collecting like terms, and solving.
- The selected level changes the question set, level label, hint language, explanation depth, and adaptive dashboard message.
- Students can switch levels at any time, making the experience suitable for mixed-ability practice.

## Learning dashboard

The dashboard tracks the number of solved questions, correct answers, and the percentage of correct responses. This gives students immediate progress feedback without storing personal information.

## Technical approach

The website is a single static HTML file containing HTML, CSS, and JavaScript. It works on computers and phones, can be opened directly in a browser, and can be deployed to GitHub Pages, Netlify, or Vercel without a build process. No database, authentication, installation, or external API key is required.

## Future AI upgrade

A production version could replace the local question bank with a server-side AI call, validate generated equations before display, store student history, and adapt difficulty from recent accuracy and response time. The prompt patterns above provide the starting contract for that upgrade.
