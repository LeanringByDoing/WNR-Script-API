# WNR Script Generator API (Render Ready)

This is a fake news script generator backend for WNR, ready for deployment on Render.com.

## 🚀 How to Deploy

1. Push this folder to a GitHub repository.
2. Go to https://render.com and create a new **Web Service**.
3. Link your repo and configure:

- Runtime: Python 3
- Build Command: `pip install -r requirements.txt`
- Start Command: `python app.py`
- Environment Variable: `OPENAI_API_KEY` → your OpenAI key

4. When live, POST to `/generate` with:

```json
{
  "station": "AL205",
  "topic": "goat mayor scandal",
  "humor": 0.7,
  "absurdity": 0.9,
  "investigative": 0.3,
  "lore": ["station000", "past"]
}
```

## ✅ Output
Returns a full fake news script structured for use in the WNR video pipeline.
