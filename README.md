# BudgetPlate (self-hosted, installable web app)
Node.js 22.13+ (built-in SQLite, nothing to compile) + Express.

## Run on your PC
    npm install
    npm start
Open http://localhost:3000

## Put it online so anyone can use it (Render example)
1. Create a free GitHub account and a new repository. Upload everything in this folder (not node_modules).
2. On render.com, choose New > Blueprint, connect that repository. Render reads render.yaml.
3. Approve the Starter plan. It includes the 1 GB disk that keeps the database safe between restarts and deploys.
4. After the deploy finishes you get an https:// link. Share it with anyone.
Without a persistent disk (the free plan), accounts are erased on every restart. Do not use the free plan for real users.

## Install on a phone
Open the link in Chrome (Android): menu > Install app. Safari (iPhone): Share > Add to Home Screen.

## Notes
- Passwords are hashed with bcrypt. Sessions last 30 days.
- Back up the database file (the DB_PATH location) regularly.
- Subscriptions are a demo toggle. Add a payment provider before charging real money.
