# reservation-dashboard
Web dashboard for managing and monitoring the restaurant reservation bot. Built with Next.js and deployed on Vercel.
# Reservation Dashboard

A web dashboard for managing and monitoring the restaurant reservation bot. Built with Next.js and deployed on Vercel. Connect it to your own fork of [reservation-bot](https://github.com/mabledong/reservation-bot) to manage your restaurants, toggle active status, trigger the bot manually, and view run logs.

## Features

- Password protected -- only you can access your dashboard
- View all your restaurants and their status
- Toggle restaurants on and off without touching the terminal
- Add and remove restaurants from a visual form
- Manually trigger the bot to run right now
- View recent bot run logs and their status

## Setup

### 1. Fork this repo

Click the Fork button in the top right on GitHub.

### 2. Deploy to Vercel

1. Go to vercel.com and sign in
2. Click **Add New Project**
3. Import your forked `reservation-dashboard` repo
4. Add the following environment variables before deploying

### 3. Set environment variables in Vercel

| Variable | Description |
|---|---|
| `GITHUB_TOKEN` | Your GitHub Personal Access Token with repo and workflow permissions |
| `GITHUB_OWNER` | Your GitHub username |
| `GITHUB_REPO` | The name of your reservation bot repo (e.g. `reservation-bot`) |
| `DASHBOARD_PASSWORD` | A password of your choice to protect the dashboard |

### 4. Get a GitHub Personal Access Token

1. Go to github.com and click your profile picture
2. Click **Settings**
3. Scroll down to **Developer settings**
4. Click **Personal access tokens** then **Tokens (classic)**
5. Click **Generate new token (classic)**
6. Give it a name like `reservation-dashboard`
7. Check **repo** and **workflow** permissions
8. Click **Generate token** and copy it immediately

### 5. Done

Once deployed, visit your Vercel URL and log in with the password you set. Connect it to your own fork of the reservation bot by setting the environment variables above.

## Built with

- Next.js
- Vercel
- GitHub API
