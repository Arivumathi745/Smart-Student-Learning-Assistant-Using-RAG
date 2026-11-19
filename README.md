
<div align="center">

# 🎓 Smart Student Learning Assistant Using RAG

### An AI-powered chatbot that answers student questions using uploaded study materials.

<img src="https://img.shields.io/badge/Python-3.10+-blue?logo=python" />
<img src="https://img.shields.io/badge/Framework-Gradio-orange" />
<img src="https://img.shields.io/badge/Vector%20Store-FAISS-green" />
<img src="https://img.shields.io/badge/AI-Nexus%20API-purple" />

</div>

---

## 📌 Project Overview

The **Smart Student Learning Assistant Using Retrieval-Augmented Generation (RAG)** is an AI-powered educational chatbot designed to help students understand and retrieve information from their study materials.

The system allows users to upload PDF documents, extracts and processes their content, converts text into numerical embeddings, and stores the embeddings in a FAISS vector database.

When a student asks a question, the system retrieves relevant information from the uploaded documents and uses a Large Language Model (LLM) through the Nexus API to generate a contextual answer.

The application provides an interactive chatbot interface using Gradio.

## 🎯 Objectives

- To develop an AI-powered student learning assistant.
- To allow students to obtain answers from uploaded PDF documents.
- To implement Retrieval-Augmented Generation (RAG).
- To perform semantic search using vector embeddings.
- To reduce the time required to search large study materials.
- To provide an interactive and user-friendly chatbot interface.

## ✨ Features

- 📄 PDF document text extraction.
- ✂️ Automatic text chunking.
- 🔢 Text embedding generation.
- 🗄️ FAISS vector storage.
- 🔍 Semantic similarity search.
- 🤖 AI-based answer generation.
- 💬 Interactive Gradio chatbot.
- 📚 Answers grounded in uploaded study material.
- 🚫 Rejection of questions unsupported by the uploaded material.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| Google Colab | Development environment |
| PyPDF | PDF text extraction |
| NumPy | Numerical operations |
| FAISS | Vector storage and similarity search |
| Nexus API | LLM and embedding API |
| nova-micro | Answer generation model |
| text-embedding-3-small | Text embedding model |
| Gradio | Frontend chatbot interface |

## 🏗️ System Architecture

```text
       Student
          |
          v
     Upload PDF
          |
          v
   PDF Text Extraction
          |
          v
      Text Chunking
          |
          v
   Embedding Generation
          |
          v
    FAISS Vector Store
          |
          |
    Student Question
          |
          v
   Question Embedding
          |
          v
    Semantic Search
          |
          v
  Relevant Text Retrieval
          |
          v
      Nexus API
          |
          v
    LLM Answer Generation
          |
          v
    Gradio Chatbot
          |
          v
    Answer to Student
```

## ⚙️ How It Works

**Step 1: PDF Upload**

The student uploads a study material PDF.

**Step 2: Text Extraction**

The system extracts text from the uploaded PDF using PyPDF.

**Step 3: Text Chunking**

The extracted text is divided into smaller chunks to make information retrieval easier.

**Step 4: Embedding Generation**

Each text chunk is converted into a numerical vector using the `text-embedding-3-small` model.

**Step 5: Vector Storage**

The generated embeddings are stored in FAISS using `IndexFlatL2`.

**Step 6: Question Processing**

The student's question is converted into an embedding.

**Step 7: Information Retrieval**

FAISS searches for the most relevant text chunks based on vector similarity.

**Step 8: Answer Generation**

The retrieved content is passed to the `nova-micro` model through the Nexus API to generate an answer.

**Step 9: Display Answer**

The generated answer is displayed through the Gradio chatbot interface.

## 📦 Installation

Install the required Python libraries:

```bash
pip install pypdf numpy faiss-cpu gradio openai
```

## 🚀 Running the Project

1. Open Google Colab.
2. Install the required dependencies.
3. Configure your Nexus API key using Google Colab Secrets.
4. Upload your study material PDF.
5. Extract and split the PDF text into chunks.
6. Generate embeddings using the Nexus API.
7. Store embeddings in FAISS.
8. Run the Gradio chatbot interface.
9. Ask questions related to the uploaded study material.

## 🔐 API Configuration

This project uses the Nexus API for text embeddings and answer generation.

Store your API key securely in Google Colab Secrets.

Secret name:

```text
NEXUS_API_KEY
```

**Important:** Never upload your API key to GitHub or expose it in source code.

## 🧪 Sample Testing

| Student Question | Expected Result |
|---|---|
| What is Artificial Intelligence? | Answer from uploaded PDF |
| Explain Narrow AI. | Answer from uploaded PDF |
| What is Machine Learning? | Answer from uploaded PDF |
| What is FAISS? | Answer from uploaded PDF |
| Explain Quantum Computing. | Information unavailable in uploaded material |

## 🎓 Applications

- Student self-learning.
- Educational assistance.
- Quick searching of study materials.
- Academic revision.
- Document-based question answering.
- Personalized learning support.

## 🔮 Future Enhancements

- Support for multiple PDF uploads.
- Chat history and conversation memory.
- Source document and page references.
- Automatic question and quiz generation.
- Summarization of study materials.
- Voice-based question answering.
- Improved retrieval accuracy.

## 👨‍💻 Project Information

**Project Name:** Smart Student Learning Assistant Using RAG

**Domain:** Artificial Intelligence and Machine Learning

**Development Environment:** Google Colab

**Frontend:** Gradio

**Backend:** Python

**Vector Database:** FAISS

**LLM:** Nexus API (`nova-micro`)

**Embedding Model:** `text-embedding-3-small`

---

## 📜 License

This project is developed for educational and academic purposes.

---

<div align="center">

### ⭐ Smart Student Learning Assistant Using RAG

**Making Learning Smarter with Artificial Intelligence!**

</div>
