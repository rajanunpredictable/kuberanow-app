# AI Social Media Studio — Kuberanow

A Streamlit canvas workspace for generating bilingual (English / Gujarati) social media slide decks with Gemini-powered backgrounds, copywriting suggestions, and an Excel export pipeline.

## Run locally

```bash
pip install -r requirements.txt
streamlit run app.py
```

App opens at `http://localhost:8501`.

## API key

The Gemini key can be entered in the sidebar at runtime, OR pre-filled via secrets:

- **Local:** create `.streamlit/secrets.toml` with `gemini_api_key = "AIzaSy..."`
- **Deployed (Streamlit Cloud):** paste the same line under **Settings → Secrets**

If no key is provided, the app runs in **Sandbox Mode** using fallback Unsplash images.

## Deploy

Push this repo to GitHub, then go to [share.streamlit.io](https://share.streamlit.io), connect the repo, and select `app.py` as the entry point. The deployed URL works on any device — install it as a PWA on Android via **Chrome → ⋮ → Add to Home screen**.
