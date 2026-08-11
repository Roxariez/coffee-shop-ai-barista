# 1. Change Directory to your folder project

```bash
cd ~/my-coffee-app

```
# 2. Setting in neccery

```bash
export PROJECT_ID=$(gcloud config get-value project)
export REGION=asia-southeast1
export GOOGLE_API_KEY="your_API_key_" (Google Ai Studio) API = Free tier

```

# 3. Run App
```bash
streamlit run app.py \
  --server.port=8080 \
  --server.address=0.0.0.0 \
  --browser.serverAddress=localhost \
  --server.enableCORS=false \
  --server.enableXsrfProtection=false
```
# ☕ Coffee Shop AI Barista

An AI-powered coffee shop chatbot built with Streamlit and Google ADK (Agent Development Kit), powered by Gemini.

## Features
- 💬 Interactive chat interface for ordering coffee and pastries
- 🎯 AI agent grounded in real menu data — recommends only items that actually exist
- ☕ Full menu display with tags (dairy-free, sugar-free, hot/cold, etc.)

## Tech Stack
- **Frontend/Backend**: Streamlit
- **AI Framework**: Google Agent Development Kit (ADK)
- **Model**: Google Gemini

## Setup

1. Install dependencies:
   \`\`\`bash
   pip install -r requirements.txt
   \`\`\`

2. Set your Gemini API key:
   \`\`\`bash
   export GOOGLE_API_KEY="your-api-key-here"
   \`\`\`

3. Run the app:
   \`\`\`bash
   streamlit run app.py
   \`\`\`

## Project Structure
- \`app.py\` — Streamlit UI and chat interface
- \`agent.py\` — AI agent logic and tool definitions
- \`menu.json\` — Coffee shop menu data (source of truth for the AI)
- \`requirements.txt\` — Python dependencies
