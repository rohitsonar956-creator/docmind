# 🧠 DocMind — Grounded AI Document Reader & RAG Workbench

![React](https://img.shields.io/badge/React-18-blue?style=flat-square&logo=react)
![Vite](https://img.shields.io/badge/Vite-6.0-646CFF?style=flat-square&logo=vite)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4-38B2AC?style=flat-square&logo=tailwind-css)
![Gemini API](https://img.shields.io/badge/Gemini_API-1.5_Flash-4285F4?style=flat-square&logo=google)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

**DocMind** is an AI-powered document reader application designed to eliminate LLM hallucinations when reading contracts, research papers, legal documents, and study material. 

It processes **PDF** and **DOCX** files, parses structured text across pages, performs client-side RAG (Retrieval-Augmented Generation) keyword/vector retrieval, and provides grounded answers backed by **exact page citations**.

---

## 🚀 Live Demo & Deployment

* **GitHub Repository:** [https://github.com/rohitsonar956-creator/docmind](https://github.com/rohitsonar956-creator/docmind)
* **Hosted Platform:** Ready for deployment on **Vercel** or **Netlify**.

---

## ✨ Features

### 📄 1. Document Extraction & Multi-Format Parsing
* **PDF & DOCX Support:** Client-side parsing retaining page boundaries and text metadata.
* **Instant Sample Testing:** Pre-loaded with realistic SLA contracts and academic survey papers for instant evaluation.
* **Multi-Stage Loading State:** Live UI feedback showing upload, extraction, semantic chunking, and assistant setup.

### 🔍 2. RAG & Anti-Hallucination Engine
* **Semantic Chunking:** Text is split into ~250-word blocks indexed by page number.
* **TF-IDF Keyword Retrieval:** Retrieves the most relevant document chunks before sending questions to the LLM.
* **Grounded Answers:** Strict system instructions prevent the model from fabricating facts or citing non-existent pages.
* **Interactive Citations:** Click any `[Page X]` badge in chat to jump straight to that page in the Reader View.

### 📊 3. Automated Document Intelligence
* **Executive Overview:** Summaries, document type classification, page count, and word count.
* **Key Takeaways:** Bullets summarizing high-priority agreements, risks, or conclusions.
* **Structured Entity Cards:** Automatic extraction of:
  * 📅 Dates & Deadlines
  * 👤 Names & Organizations
  * 🔢 Financials & SLA Metrics
  * 🛡️ Compliance Requirements & Rules

### 🎓 4. Interactive Study Mode
* **3D Flip Flashcards:** Flip through question-and-answer revision cards generated directly from the text.
* **Revision Study Notes:** Concise bullet points covering essential topics for quick review.

### 💻 5. Professional 3-Column SaaS Workbench
* **Navigation Column:** Page index thumbnails with quick preview snippets.
* **Main Intelligence Workspace:** Tabs for Overview, Entity Cards, Study Mode, and Reader View.
* **AI Q&A Panel:** Live chat assistant with preset prompt pills and citation links.

---

## 🛠️ Tech Stack

* **Frontend Framework:** React 18 (Vite)
* **Styling:** Tailwind CSS + Lucide React Icons
* **Document Parsing:** `pdfjs-dist`, `mammoth` (DOCX extraction)
* **Retrieval Engine:** Custom Client-Side TF-IDF RAG Search
* **AI Integration:** Google Gemini 1.5 Flash API

---

## 📂 Project Structure
