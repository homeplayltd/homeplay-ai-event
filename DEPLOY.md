# Deploy to Vercel

## Option 1: One-command deploy (no GitHub needed)

```bash
cd "path/to/web-app"
npx vercel --prod
```

Follow the prompts — it will ask you to log in (if needed), confirm the project name, and deploy.

## Option 2: Via GitHub + Vercel

1. Create a GitHub repo and push:

```bash
cd "path/to/web-app"
git init
git add -A
git commit -m "Homeplay AI for Interior Designers web app"
gh repo create homeplay-ai-event --public --source=. --push
```

2. Connect to Vercel:
   - Go to https://vercel.com/new
   - Import the `homeplay-ai-event` repo
   - Framework preset: **Other**
   - Output directory: `.`
   - Click Deploy

That's it — future pushes to `main` will auto-deploy.
