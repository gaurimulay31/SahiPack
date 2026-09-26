# SahiPack — Smart Food Label Analysis & Personalized Insight Web Application

> **Tagline**: *"Don’t just read the label. Understand it."*

https://sahipack-app.web.app

## What is SahiPack?
**SahiPack** is a responsive, independent packaged food label analysis web application designed to help consumers evaluate food products using barcode scanning, label image OCR, general food quality scoring on a strict **0–10 scale**, multi-select personalization matching (age groups, allergies, health requirements, lifestyle goals), personalized scoring on a **0–10 scale**, score explanations ("Why This Score?"), better-suited Indian food alternatives, an AI assistant ("Ask SahiPack"), and future feature showcases.

## Core Features
1. **0–10 General Food Quality Score**: Deterministic evaluation of sugar, sodium, saturated fat, protein, fiber, NOVA processing classification (1-4), Nutri-Score, and additives on a 0.0 to 10.0 scale.
2. **Multi-Select Personalization Engine**: Customize profile across Age Groups (0-3, 3-18, 18-35, 35-60, 60+), Dietary Preferences, Allergies (including custom "Other" text input), Health Requirements (Diabetes, Hypertension, Heart Disease, Weight Loss, Kidney Health), and Lifestyle Goals (High Protein, Clean Eating, Low Carb, Gut Health).
3. **0–10 Personalized Food Score**: Adjusts general score to user profile and flags allergen warnings.
4. **"Why This Score?" Explanations**: Transparent breakdown of positive and score-reducing factors.
5. **Better-Suited Indian Market Alternatives**: Recommends healthier food products in similar categories.
6. **Barcode Scanner & Label Image Upload**: WebRTC camera scanner + simulated OCR label text extraction.
7. **Ask SahiPack AI**: Conversational food query assistant.
8. **Responsive Mobile-to-Desktop Layout**: Tested and optimized across 360px, 390px, 768px, 1024px, 1366px, and 1440px viewport widths.

## Technology Stack
- **Frontend**: HTML5, CSS3 (Flexbox/Grid, Custom Properties, Responsive Containers), Vanilla JavaScript (ES6+ modular controllers)
- **Backend API**: Python 3.11+ / Flask Framework
- **Database**: SQLite / Open Food Facts REST API
- **Scoring Engine**: Rule-based deterministic 0–10 score calculator (`ml/scoring/score_calculator.py`)

## Running Locally
```bash
# Start Flask Backend & Serve Frontend
.venv\Scripts\python.exe backend/app.py
```
Open browser at `http://127.0.0.1:5000/`.
