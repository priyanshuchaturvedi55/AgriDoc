# 🌿 AgriDoc: AI Plant Disease Detector

**AgriDoc** is an AI-powered web application designed to help farmers and plant enthusiasts quickly identify plant diseases from leaf images. By leveraging the power of Google Gemini AI, it provides accurate disease diagnoses, severity assessments, and actionable treatment recommendations.

🚀 **Live Deployment:** [https://agridoc-app.onrender.com/index](https://agridoc-app.onrender.com/index)

---

## ✨ Features

- **AI Disease Detection:** Upload an image of a plant leaf, and the Google Gemini Vision model will analyze it to detect diseases or confirm if the plant is healthy.
- **Treatment Recommendations:** Get detailed descriptions of the disease, its severity, and steps to prevent or treat it.
- **Supplement Recommendations:** Built-in marketplace linking to relevant supplements and treatments based on the diagnosed issue.
- **Cloud-Optimized Backend:** Built with a lightweight Flask architecture and custom fallback mechanisms to run smoothly on cloud platforms like Render.
- **Responsive UI:** Clean, mobile-friendly interface built with Bootstrap 5.

## 🛠️ Tech Stack

- **Backend:** Python, Flask
- **AI Integration:** Google Gemini AI API (`gemini-2.5-flash`)
- **Data Processing:** Pandas
- **Frontend:** HTML5, CSS3, Bootstrap 5
- **Deployment:** Render, Gunicorn

## 🚀 Getting Started (Local Development)

### 1. Clone the repository
```bash
git clone https://github.com/priyanshuchaturvedi55/AgriDoc.git
cd AgriDoc
```

### 2. Install Dependencies
Make sure you have Python installed. Then run:
```bash
pip install -r requirements.txt
```

### 3. Environment Variables
You need a Google Gemini API Key to use the AI features. Set it as an environment variable:
```bash
# On Windows
set GEMINI_API_KEY=your_api_key_here

# On Mac/Linux
export GEMINI_API_KEY=your_api_key_here
```

### 4. Run the Application
Navigate to the main application directory and start the Flask server:
```bash
cd AgriDoc/main_app
python app.py
```
The application will be accessible at `http://localhost:5000` or `http://127.0.0.1:5000`.

## 📂 Project Structure

- `AgriDoc/main_app/app.py`: Main Flask application handling routing and AI integration.
- `AgriDoc/main_app/templates/`: HTML templates for the frontend.
- `AgriDoc/main_app/static/`: CSS, images, and uploaded files.
- `disease_info.csv` & `supplement_info.csv`: Datasets used for fallback operations and supplement recommendations.
