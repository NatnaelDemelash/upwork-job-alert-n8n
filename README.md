# ⚡ Upwork Job Alert — n8n Automation

Automatically finds fresh Upwork jobs matching your skills, filters them with
Groq AI, and sends clean alerts to your Telegram. Runs every 2 hours.
Completely free to run.

## 📸 Preview

[Add screenshot of your Telegram alert here]

## 🔧 How It Works

1. **SerpApi** searches Google for fresh Upwork jobs across 4 categories
2. **Filter node** removes jobs older than 48 hours
3. **Groq AI (Llama 3.3)** reads each job and decides GOOD or BAD
4. **Telegram Bot** sends a clean alert for every GOOD job

## 🛠 Tech Stack

- [n8n](https://n8n.io) — workflow automation
- [SerpApi](https://serpapi.com) — Google job search (250 free/month)
- [Groq API](https://groq.com) — free Llama 3.3 AI filtering
- Telegram Bot API — free alerts

## 💰 Cost

| Tool              | Cost             |
| ----------------- | ---------------- |
| n8n (self-hosted) | Free             |
| SerpApi           | Free (250/month) |
| Groq API          | Free             |
| Telegram          | Free             |
| **Total**         | **$0/month**     |

## 🚀 Setup

1. Import `workflow.json` into your n8n instance
2. Add your SerpApi API key
3. Add your Groq API key
4. Create a Telegram bot via @BotFather
5. Add your Telegram Chat ID
6. Activate the workflow

## 📬 Alert Format

Each alert includes job title, description snippet, posted date,
and a direct Apply Now link.

## ⚠️ Security Note

Before importing this workflow, add your own:

- SerpApi API key (free at serpapi.com)
- Groq API key (free at console.groq.com)
- Telegram Bot token + your Chat ID

## 👤 Built By

**Natnael Demelash** — React Developer & n8n Automation Specialist
[Upwork Profile](https://www.upwork.com/freelancers/~01ddf1eafb3a557e61)

```

---

**For your Telegram Bot profile picture — here's what to set:**

1. Message **@BotFather**
2. Send `/mybots`
3. Select `@upwork_alert_natnael_bot`
4. Click **Edit Bot → Edit Botpic**
5. Upload an image

For the image, use any of these free options:
- Go to **canva.com** → create a 512x512 image
- Dark background + ⚡ lightning bolt icon + text "Job Alert"
- Use green (#2D9E5F) and white colors to match Upwork's vibe

**Bot description to set in BotFather:**
```

⚡ Your personal Upwork job alert bot.
Sends AI-filtered job matches directly to you every 2 hours.
Built with n8n + Groq AI.
