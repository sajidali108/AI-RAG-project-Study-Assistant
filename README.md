# 🎓 AI Study Assistant (RAG)
### *Bridging the gap between complex documents and instant answers.*

---

## 👋 Overview
Welcome! This project is a **Retrieval-Augmented Generation (RAG)** application designed to act as a personal study companion. It allows users to upload dense academic materials (like PDFs) and interact with them using natural language. 

Instead of scrolling through hundreds of pages to find a single definition, you can simply ask a question and get a precise answer based specifically on your documents.

## 🚀 Key Features
* **Intelligent Document Parsing**: Automatically extracts and processes text from PDF files using `pypdf`.
* **Context-Aware Retrieval**: Uses advanced text-splitting techniques to break down information into manageable "chunks," ensuring the AI maintains focus and accuracy.
* **Local LLM Integration**: Built to work with **Ollama** (specifically `llama3.2`), ensuring high performance and data privacy by running the model locally.
* **Human-Like Interaction**: A seamless flow where the system retrieves the most relevant snippets of text before generating a natural, easy-to-understand response.

## 🛠️ Tech Stack
* **Orchestration**: `LangChain` (Core, Community, and Text-Splitters)
* **Models**: Ollama (`llama3.2`)
* **Data Handling**: `PyPDF` for document loading
* **Environment**: Jupyter Notebook / Google Colab

## 📖 How It Works
1.  **Ingestion**: You provide a PDF document (textbook, research paper, or notes).
2.  **Chunking**: The system breaks the text into smaller segments so the AI doesn't get "overwhelmed" by long chapters.
3.  **Vectorization**: The text is converted into a format the computer can search mathematically.
4.  **Querying**: You ask a question in plain English.
5.  **Retrieval & Generation**: The app finds the exact paragraph containing your answer and uses the LLM to explain it to you simply.

## ⚙️ Setup & Installation
To get this running on your local machine:

1.  **Install Dependencies**:
    ```bash
    pip install langchain langchain-community pypdf
    ```

2.  **Set Up Ollama**:
    * Install [Ollama](https://ollama.com/).
    * Pull the required model:
        ```bash
        ollama run llama3.2
        ```

3.  **Run the Notebook**:
    * Open `AI Study Assistant (RAG).ipynb` in VS Code or Jupyter.
    * Follow the cells to initialize the RAG chain and start chatting with your documents!

## 🌟 Future Enhancements
* **Vector Database Integration**: Adding ChromaDB or FAISS for permanent, high-speed document storage.
* **Web Interface**: Developing a frontend with **Streamlit** for a more polished user experience.
* **Multi-Format Support**: Expanding beyond PDFs to support Word docs, PowerPoints, and even YouTube transcripts.

---
*Developed with a focus on making learning more accessible and efficient.*
