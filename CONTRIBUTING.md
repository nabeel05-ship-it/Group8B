# Contributing to FoodWise (Group8B)

## Branches
- `main` is the stable branch. Don't commit to it directly. All changes go in through a Pull Request.
- Each member works on their own branch, named after them (for example `nabeel`).

## First-time setup
```bash
git clone https://github.com/nabeel05-ship-it/Group8B.git
cd Group8B
npm install
cp .env.example .env.local   # fill in your own values; never commit this file
git checkout -b <your-name>
git push -u origin <your-name>
```

## Daily workflow
```bash
git checkout <your-name>
git pull origin main          # stay up to date with main
# ...make changes...
git add <files>
git commit -m "feat: short description"
git push
```
Then open a Pull Request from `<your-name>` into `main` on GitHub and ask a teammate to review it.

## Secrets
- Never commit `.env`, `.env.local`, API keys, database passwords or other credentials.
- Only `.env.example`, with empty values, belongs in the repo.
- If you commit a secret by mistake, tell the team right away and rotate (change) the key. Deleting the file in a later commit does not remove it from Git history.
