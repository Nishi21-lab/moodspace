# 🌅 MoodSpace

A simple, single-file web app for tracking your daily mood, journaling your thoughts, and seeing how your emotional state changes over time — with a touch of community feel through a simulated "World Mood" feed.

## What is MoodSpace?

MoodSpace is a lightweight mood-journaling app built entirely in HTML, CSS, and JavaScript — no backend, no build tools, no dependencies to install. Just open the file in a browser and start logging how you feel.

Each time you check in, MoodSpace gives you a short motivational quote tailored to your mood, logs your entry to a personal history you can revisit, and updates a community-style "World Mood" view so you can see how today's check-ins (including your own) are trending.

## Features

- **Daily mood check-in** — Pick from five moods (Awful, Sad, Okay, Good, Great) and add a free-text note about what's on your mind.
- **Personalized motivation** — After saving an entry, you get a random quote matched to your current mood.
- **My History** — A line chart (powered by Chart.js) visualizing your mood scores over your last 14 entries, plus a scrollable list of your past check-ins.
- **World Mood** — A live-feeling feed of recent check-ins and aggregate stats (today's check-in count, dominant mood, and percent feeling good) based on data stored in your browser.
- **No sign-up, no server** — Everything runs client-side and persists via `localStorage`, so your data stays in your own browser.

## Tech Stack

- Plain HTML, CSS, and vanilla JavaScript
- [Chart.js](https://www.chartjs.org/) (loaded via CDN) for the mood history graph
- `localStorage` for persistence — no database or backend required

## Getting Started

1. Clone or download this repository.
2. Open `index.html` in any modern web browser.
3. Start logging your mood!

No build step, no `npm install`, no server setup needed.

## How It Works

- Personal entries are saved under the `moodspace_personal_v1` key in `localStorage`.
- Simulated community entries are saved under `moodspace_world_v1`.
- The "World Mood" tab is illustrative — since there's no backend, the community feed only reflects check-ins made from your own browser, not real users elsewhere. This is meant as a demo of what a real-time community mood feed could look like; wiring it up to a real backend (e.g. Firebase, Supabase, or a custom API) would be a natural next step for anyone forking this project.

## Possible Improvements / Ideas for Contributors

- Connect "World Mood" to a real shared backend so check-ins are visible across users.
- Add data export (CSV/JSON) for personal mood history.
- Add authentication so history syncs across devices.
- Add weekly/monthly mood summaries or streak tracking.
- Add light/dark theme toggle.

## License

This project is open source. Feel free to add a license of your choice (MIT is a common, permissive option for projects like this).

## Disclaimer

MoodSpace is a personal journaling tool and is not a substitute for professional mental health support. If you're struggling, please reach out to a mental health professional or a crisis line in your area.
