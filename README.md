
# Prizm - Created for: ACM hackventure 1.0 (January, 2025)
## Empowering Visually Impaired Users with Legal & Medical Document Accessibility

Prizm is an innovative web application designed to empower visually impaired individuals by providing real-time, AI-powered guidance to navigate complex legal and medical documents. With easy document scanning, simplified summaries, and an AI chatbot for support, Prizm makes understanding intricate legal and medical terminology accessible, restoring confidence, independence, and empowerment to visually impaired users.

### Key Features
#### 1. Seamless Document Scanning
Capture documents easily using your phone’s camera. Real-time visuals and alignment feedback ensure clear scans every time.

#### 2. Advanced Text Extraction and Privacy
Prizm uses robust Optical Character Recognition (OCR) to convert scanned documents into editable, shareable text. Sensitive information is automatically filtered using regex-based masking to protect user privacy.

#### 3. Simplified Summarization
Complex legal and medical jargon is transformed into clear, concise language, helping users make informed decisions without confusion.

#### 4. AI-Powered Chatbot
A secure, context-aware chatbot is available 24/7 to answer questions about workplace rights, Indian laws, medical terminology, or any related concerns. User privacy and data security are prioritized at every step.

#### 5. Accessibility by Design
Prizm incorporates text-to-speech, high-contrast visuals, adjustable font sizes, multilingual support, and keyboard navigation to ensure usability for all users, regardless of their specific needs.

#### 6. Real-Time Voice Control
Users can navigate the app and interact with the chatbot using voice commands, reducing dependence on touchscreens or keyboards.

### Project Structure
This repository includes:

#### Frontend
1. index.html — Home page with voice-enabled navigation.
2. camera.html — Live document scanning with a real-time feed and summarization.
3. chatbot.html — Voice-enabled AI chatbot for legal and medical queries.
4. styles.css — Unified styling for an accessible, high-contrast user interface.
5. scripts.js — Supporting client-side JavaScript for interaction and controls.
6. upload.html - Interactive upload page for OCR, AI summarization, and voice playback.


#### Backend
1. camera.py — Handles real-time camera feed and captures frames.
2. regex.py — Processes extracted text and applies masking for sensitive information.
3. test.py —  Provides endpoints to scan documents via webcam or upload, extracts text with OCR, and summarizes using Gemini AI.

### Getting Started

#### Prerequisites
- Python 3.11 or higher
- pip (Python package manager)

#### Installation & Running the Application

1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd Prizm
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Backend Server**
   ```bash
   python backend/camera.py
   ```

4. **Access the Home Page**
   - Open your web browser and navigate to: `http://localhost:5000`
   - The home page (index.html) will load automatically
   - You can then navigate to Camera Scanning, Chatbot, or Upload pages from the home page

#### Application URLs
- **Home Page**: `http://localhost:5000/` or `http://localhost:5000/index.html`
- **Document Scanning**: `http://localhost:5000/camera.html`
- **AI Chatbot**: `http://localhost:5000/chatbot.html`
- **Document Upload**: `http://localhost:5000/upload.html`

### Accessibility Commitments
1. High-contrast color palette and adjustable font sizes
2. Text-to-speech for all content and summaries
3. Voice commands for site navigation and chatbot interaction
4. Semantic HTML with ARIA labels and skip links for screen readers

#### Test
