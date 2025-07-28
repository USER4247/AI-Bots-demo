# 🤖 Reddit Bot with Gemini + PRAW

A minimal Reddit comment bot powered by Google's Gemini LLM (via Generative Language API) and [PRAW](https://praw.readthedocs.io/) (Python Reddit API Wrapper). This bot analyzes Reddit posts and generates thoughtful replies. Entirely built and run within Google Colab.

---

## ⚠️ Disclaimer

This project is for **demonstration purposes only**. It is not intended for production or industrial usage.

If you're interested in **enhanced, robust, and scalable versions** of this software, feel free to **raise an issue** or contact the maintainer.

---


## 🚀 Features

- 🔍 Scans specific subreddits using keyword or condition filters
- 🧠 Uses Gemini LLM to generate high-quality, nuanced comments
- ⚡ Runs inside Colab—no installation or local setup needed
- 🔁 Can loop continuously or run once per execution
- 📝 Easily tweak prompt to change tone or behavior

---

## 🛠️ Setup & Usage

### 1. Open the Notebook
You can open the `.ipynb` file directly in [Google Colab](https://colab.research.google.com/) from this repo.

### 2. Add Your Credentials
Create a `config.json` file with the following format:

```json
{
  "reddit_client_id": "YOUR_REDDIT_APP_ID",
  "reddit_client_secret": "YOUR_REDDIT_SECRET",
  "reddit_username": "YOUR_USERNAME",
  "reddit_password": "YOUR_PASSWORD",
  "user_agent": "your-bot-name",
  "gemini_api": {
    "api_key": "YOUR_GEMINI_API_KEY"
  }
}
```

You can upload it in Colab using the upload widget or mount Google Drive.

### 3. Run the Notebook
Click "Runtime > Run all". The bot will:
- Authenticate with Reddit
- Search for matching posts/comments
- Use Gemini to craft replies
- Post back to Reddit using PRAW

---

## 🧠 Customization

- Modify the prompt template to change the personality or tone.
- Adjust filters to target specific subreddits or post types.
- Add conditions (like number of upvotes or keywords) before replying.

---

## 💡 Notes

- Gemini API has usage quotas and may need a billing account.
- Reddit has rate limits—use `time.sleep()` to avoid bans.
- Always test bots in private subreddits or via `dry_run=True` mode.

---

## 📜 License

MIT License

---

## 🙏 Acknowledgements

- [Google Generative Language API](https://ai.google.dev/)
- [PRAW: Python Reddit API Wrapper](https://praw.readthedocs.io/)
- [Google Colab](https://colab.research.google.com/)
- Built with ❤️ and lots of trial & error

---

If this project helped you, drop a ⭐ on GitHub or fork it and make it your own!
