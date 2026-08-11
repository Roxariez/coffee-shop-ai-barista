# 1. เข้าไปที่โฟลเดอร์โปรเจกต์
cd ~/my-coffee-app

# 2. ตั้งค่าตัวแปรที่จำเป็น
export PROJECT_ID=$(gcloud config get-value project)
export REGION=asia-southeast1
export GOOGLE_API_KEY="ใส่_API_key_ของคุณตรงนี้"

# 3. รันแอป
streamlit run app.py \
  --server.port=8080 \
  --server.address=0.0.0.0 \
  --browser.serverAddress=localhost \
  --server.enableCORS=false \
  --server.enableXsrfProtection=false

# 1. เข้าไปที่โฟลเดอร์โปรเจกต์
cd ~/my-coffee-app

# 2. ตั้งค่าตัวแปรที่จำเป็น
export PROJECT_ID=$(gcloud config get-value project)
export REGION=asia-southeast1
export GOOGLE_API_KEY="ใส่_API_key_ของคุณตรงนี้"

# 3. รันแอป
streamlit run app.py \
  --server.port=8080 \
  --server.address=0.0.0.0 \
  --browser.serverAddress=localhost \
  --server.enableCORS=false \
  --server.enableXsrfProtection=false

  เรื่องที่ 2: กด "Add a README"

กดปุ่มสีเขียว "Add a README" ได้เลยครับ ระบบจะพาไปหน้าสร้างไฟล์ ให้วางเนื้อหานี้ลงไป:
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
