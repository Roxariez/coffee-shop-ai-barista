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
