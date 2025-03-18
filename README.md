# Student Exam Buddy 📚

An AI-powered study companion that helps students prepare for exams through intelligent document search, video summarization, and automated question generation.

---

## 🌟 Features

- **📖 Document Search**: Upload and query study materials (PDFs) using natural language.
- **🎥 Video Summarizer**: Get concise summaries of educational YouTube videos.
- **📝 MCQ Generator**: Automatically generate multiple-choice questions from study materials.
- **📄 Essay Questions**: Create long-form questions with model answers for practice.

---

## 🛠️ Tech Stack

- **Agentic Framework**: [Agno](https://www.agno.com/)
- **Frontend & App Framework**: [Streamlit](https://streamlit.io/)
- **AI Models**:
  - [OpenAI GPT-4o](https://openai.com) for chat functionality and question generation.
  - [Google Gemini](https://ai.google.dev/) for YouTube video summarization.
- **Vector Database**: [LanceDB](https://lancedb.com/) for efficient document retrieval.
- **Document Processing**: PDF extraction and vectorization.

---

## 📋 Prerequisites

- Python 3.9+
- OpenAI API key (for GPT-4o and embeddings)
- Google API key (for Gemini model)

---

## ⚙️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/anil2k/Student-Exam-Buddy
   cd Student-Exam-Buddy
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file with your API keys:
   ```
   GOOGLE_API_KEY=your_google_api_key
   OPENAI_API_KEY=your_openai_api_key
   ```

---

## 🚀 Usage

1. Start the application:
   ```bash
   streamlit run main.py
   ```

2. Open your browser and go to `http://localhost:8501`

3. Navigate through the tabs to access different features:
   - **Chat Assistant**: Ask questions about uploaded documents.
   - **Video Summarizer**: Get summaries of YouTube lectures.
   - **MCQ Generator**: Create multiple-choice questions for practice.
   - **Long Questions**: Generate essay-style questions.

---

## 🗂️ Project Structure

```
student-exam-buddy/
├── .env                  # Environment variables and API keys
├── .gitignore            # Git ignore file
├── main.py               # Main application file
├── tmp/                  # Temporary storage directory
│   └── lancedb/          # LanceDB database files
└── uploaded_docs/        # Directory for storing uploaded PDFs
```

---

## 📝 How It Works

### 1. **Document Processing**
- Upload PDFs via the sidebar.
- Documents are vectorized and stored in LanceDB.
- The knowledge base enables semantic search for relevant information.

### 2. **Chat Interface**
- Ask questions about study materials.
- AI agent retrieves relevant answers from the knowledge base.
- Get contextual responses based on uploaded documents.

### 3. **YouTube Summarization**
- Enter a YouTube URL.
- Gemini AI processes video content.
- Receive structured summaries with key insights.

### 4. **Question Generation**
- Generate MCQs with adjustable difficulty levels.
- Create long-form questions with model answers.
- Questions are based on uploaded study materials.

---

## 🔒 API Key Security

- Keep API keys confidential.
- Never expose the `.env` file.
- Be aware of API usage costs.

---

## 🤝 Contributing

Contributions are welcome! Feel free to submit a pull request.

---

## 📜 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

