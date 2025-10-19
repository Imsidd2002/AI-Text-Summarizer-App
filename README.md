# 🧠 AI Text Summarizer App

## 📝 Introduction
This repository contains a **Node.js** application designed to summarize text using the **Hugging Face API**.  
It provides a service to generate concise summaries of long texts — taking a text input and returning a summarized version.

This project is ideal for:
- Developers looking to integrate text summarization into their applications.
- Anyone interested in exploring the **Hugging Face API** for **Natural Language Processing (NLP)** tasks.

---

## ⚡ Overview
The app exposes a simple API endpoint that accepts a block of text and returns its summarized version using Hugging Face models.  
It’s lightweight, fast, and easy to integrate into any backend system.

---

## 🚀 Quick Start

Follow these steps to get started quickly:

1. **Clone the repository**
   ```bash
   git clone https://github.com/Imsidd2002/AI-Text-Summarizer-App
   ```

2. **Navigate to the project directory**
   ```bash
   cd AI-Text-Summarizer-App
   ```

3. **Install dependencies**
   ```bash
   npm install
   ```
   *(or use `yarn install` if you prefer Yarn)*

4. **Set your Hugging Face API key**

   Obtain an API key from [Hugging Face](https://huggingface.co/settings/tokens)  
   Then set it as an environment variable:

   ```bash
   export ACCESS_TOKEN="YOUR_API_KEY"
   ```

   Alternatively, create a `.env` file in the root directory:
   ```
   ACCESS_TOKEN=YOUR_API_KEY
   ```

5. **Run the application**
   ```bash
   node index.js
   ```

   By default, the server starts on **port 3000**.

6. **Test the summarization endpoint**

   You can test it using **curl**, **Postman**, or any API client:

   ```bash
   curl -X POST http://localhost:3000/summarize    -H "Content-Type: application/json"    -d '{"text_to_summarize": "Your long text here..."}'
   ```

---

## 📁 Repository Structure

```
AI-Text-Summarizer-App/
├── index.js          # Main application file (Express server setup, route definition)
├── summarize.js      # Contains the summarization logic and Hugging Face API interaction
├── public/           # Directory for serving static content (optional front-end)
├── package.json      # Project dependencies and metadata
└── README.md         # This documentation file
```

---

## 🧩 Prerequisites

### Required Software
- **Node.js** (v16 or later recommended)  
- **npm** or **yarn** (package manager)  
- **Hugging Face API key** (get it [here](https://huggingface.co/settings/tokens))  
- A code editor or IDE (e.g., **VS Code**, **Sublime Text**)

### Knowledge Needed
- Basic understanding of **JavaScript** and **Node.js**
- Familiarity with **HTTP requests (GET, POST)**
- Understanding of **environment variables**
- *(Optional)* Basic front-end knowledge (**HTML, CSS, JS**) if extending UI

---

## 🧠 Example Request & Response

**Request:**
```json
{
  "text_to_summarize": "Artificial Intelligence is transforming industries by automating tasks, improving decision-making, and enhancing productivity..."
}
```

**Response:**
```json
{
  "summary": "AI automates tasks and enhances decision-making to boost productivity across industries."
}
```

---

## 🧑‍💻 Author
**Siddharth Thakur**  
📍 Mumbai, India  
🔗 [GitHub Profile](https://github.com/Imsidd2002)

---

## 📜 License
This project is licensed under the **MIT License**.  
Feel free to use, modify, and distribute it with attribution.

---

⭐ **If you find this project helpful, give it a star on GitHub!**
