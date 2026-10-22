# Firstweek · Prototype 02

Firstweek is a prototype you can try: onboarding where the company sets up a new hire's first week, and the new hire gets answers only from the company's own documents, with the source, and a person when the documents don't know.

Concept and design by [Victor Mascaro](https://victor-mascaro-ux.github.io/my-portfolio/), UX/AI designer.

**Live prototype:** https://victor-mascaro-ux.github.io/firstweek/

## The problem

47% of digital workers struggle to find the information they need to do their jobs. Source: [Gartner survey](https://www.gartner.com/en/newsroom/press-releases/2023-05-10-gartner-survey-reveals-47-percent-of-digital-workers-struggle-to-find-the-information-needed-to-effectively-perform-their-jobs) of 4,861 full-time digital workers in the US, UK, India and China, May 2023.

## How to try it

The bar above the browser window walks you through 7 short tasks on two laptops: first Omar, on Acme's People team, sets up Nina's first week; then Nina, a new hire in sales, asks questions. Each task has a **Show me** button that does it for you, and if you pause for a few seconds, a pulsing outline points at the next click. Each part shows a different thing the AI does:

1. **The draft**: the AI drafts the first week from Acme's documents, and every step links to the passage it came from.
2. **The company's own steps**: Omar moves the VPN to day 1 (drag it, or use the step's menu) and adds a lunch with a buddy. The AI drafts; the People team decides.
3. **Answers with sources**: Nina asks when to pick a health plan. The answer cites the benefits guide, and the number opens the exact passage.
4. **Documents that disagree**: the handbook says 15 vacation days, a newer update says 20. The answer shows both and goes with the newer one.
5. **"I don't know"**: nothing in the documents covers dogs at the office, so the AI says so and hands the question to Jordan, Nina's manager.
6. **Answers that stay**: Jordan's answer goes back to Omar, who adds it to the handbook for the next new hire.

## Design decisions

- **Every answer shows its source.** Click the number to read the exact passage, and see when it was last updated.
- **Documents disagree? It says so.** It shows both, and goes with the newer one.
- **"I don't know" is an answer.** When the documents don't cover it, the AI hands you to your manager instead of guessing.
- **The company owns the steps.** The AI drafts the first week from your documents; the People team makes it its own.

## What's real

- The AI is scripted on five sample documents, so it works the same for everyone. A question it doesn't recognize gets the honest "I couldn't find this" answer.
- There's no backend, no analytics and no API key. Nothing you type leaves your browser.
- Firstweek, Acme, Omar Haddad (People team), Nina Costa (a new hire in sales), Jordan Lee (Nina's manager) and Acme's documents are all fictional.
- English and Brazilian Portuguese, picked from your browser language.
- The app adapts to the window: on a phone it takes the full screen.

## Run it locally

Open `index.html` in a browser. It's a single static file with no build step.
