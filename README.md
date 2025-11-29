# Multilingual Document Q&A System

A full-stack web application that allows users to upload PDF documents and ask questions in **multiple languages**.  
The system uses **AI Question Answering + Translation Pipeline** to generate accurate, multilingual answers.

---

## Features

- **PDF Upload** (Recommended: 10–15 pages)
- **Automatic Text Extraction**
- **Multilingual Question Support** (8+ languages):
  - English, Hindi, Gujarati, Marathi, Tamil, Bengali, Kannada, Telugu
- **AI-Powered Q&A** using **Groq LLaMA 3.3 / 8B / 70B models**
- **Automatic Language Detection**
- **End-to-End Translation Pipeline**
  - Question → English  
  - Model Answer → English  
  - Final Answer → User's Language
- **Clean & Responsive UI**

---

## Tech Stack

### **Backend**
- Python 3.8+
- Flask
- PyPDF2 (PDF text extraction)
- langdetect (language identification)
- deep-translator (translation)
- Groq API — LLaMA 3.3 / LLaMA 3.1 Instant Models (FREE)

### **Frontend**
- HTML5
- CSS3
- JavaScript (Vanilla)

---

## Prerequisites

- Python **3.8 or higher**
- A **Groq API Key** (free)
- pip installed on your system

---

## Installation

### **1. Create Project Structure**
```bash
Multilingual_QA_Project/
├── src/
│   ├── app.py                 # Flask main application
│   ├── pdf_processor.py       # Extracts text from uploaded PDFs
│   ├── translator.py          # Handles language translation (input & output)
│   ├── qa_engine.py           # Groq LLM-powered Question Answering logic
│
│   ├── templates/
│   │   └── index.html         # Frontend UI (HTML)
│
│   └── static/
│       ├── style.css          # Styling for the UI
│       └── script.js          # Frontend JavaScript for form handling & AJAX
│
├── uploads/                   # Temporary storage for uploaded PDFs
├── sample_pdfs/               # Sample PDFs for testing
├── screenshots/               # Screenshots of the application UI
│
├── requirements.txt           # All Python dependencies
├── .env                       # Environment variables (Groq API key)
└── README.md                  # Project documentation

```

### **2. Create virtual environment**
```bash
python -m venv venv
# Activate:
# Windows:
venv\Scripts\activate
```

### **3. Install dependencies**
```bash
pip install -r requirements.txt
```

### **4. Get Groq API Key**
```bash
from https://console.groq.com/
```

### **5. Create .env file**
Create a .env file in the project root:
```bash
GROQ_API_KEY=gsk__actual_key
```

## Running the Application
```bash
cd src
python app.py
```
Open browser and navigate to: http://localhost:5000

