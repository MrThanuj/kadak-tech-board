# Kadak Tech Referral Board 📌❤️

A simple shared board for the Kadak Tech community to post referrals and job hunts, so asks don't get lost in the group chat.

**Live site:** https://mrthanuj.github.io/kadak-tech-board/

## What it does

- **Refer** — people open to referring list their company and whether they're currently taking referrals
- **Job Seekers** — folks list their target company, role, and status (Looking → Interviewing → Referred → Placed)
- **Wins** — a running list of everyone who's landed something 🎉
- **Guide** — quick how-to, plus a button to export a backup of the board as JSON

## How it's built

- A single static `index.html` file — no build step, no framework, just HTML/CSS/vanilla JS
- Data is stored in a free [Firebase Realtime Database](https://firebase.google.com/products/realtime-database), read and written directly from the browser via its REST API
- No login system — anyone with the link can view and add/edit entries. Simple by design, but that also means please only edit your own listings

## Running it locally

Clone the repo and open `index.html` in a browser, or serve it with any static server:

```bash
git clone https://github.com/mrthanuj/kadak-tech-board.git
cd kadak-tech-board
python3 -m http.server
```

It'll talk to the same shared Firebase database as the live site, so be mindful while testing (or point it at your own Firebase project's URL at the top of the `<script>` section if you want a sandbox to experiment in).

## Want to contribute?

Very welcome! Ideas, bug fixes, design tweaks, new features, all appreciated. Some thoughts on what might be worth adding:

- Light way to reduce spam/abuse on a fully open board
- Notifications or a "watch this company" feature
- Better mobile layout polish
- Anything else you think would help the group

To contribute:
1. Fork the repo
2. Make your changes to `index.html`
3. Open a pull request with a short description of what you changed and why

If you're not comfortable with git/GitHub, no worries — just message in the group with your idea and I'll help get it in.

## A couple of honest limitations

- The board is fully open (no auth), so please be respectful of others' entries
- It's a small side project, not a polished product, so expect some rough edges
- Feedback and suggestions are genuinely welcome, this is meant to evolve with what the community actually needs
