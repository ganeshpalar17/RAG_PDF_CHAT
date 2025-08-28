🚀 Features

Upload any PDF file

Extracts text and splits it into chunks

Stores embeddings in a FAISS vector database

Ask questions in plain English

Get accurate, context-based answers

Interactive Streamlit UI

RAG_DOCUMENT_CHAT/
│── faiss_index/ # Stores FAISS index (vector DB)
│── .env # Environment variables (Google API key)
│── .gitignore # Ignored files for Git
│── apoi.txt # (Optional) backup file
│── pdfchat.py # Main Streamlit app
│── README.MD # Documentation
│── requirements.txt # Dependencies

1️⃣ Clone the Repository

git clone https://github.com/Ganeshpalar/RAG_DOCUMENT_CHAT.git
cd RAG_DOCUMENT_CHAT

2️⃣ Create a Virtual Environment
python -m venv venv

# Activate it:

# On Windows:

venv\Scripts\activate

# On Mac/Linux:

source venv/bin/activate

3️⃣ Install Dependencies
pip install -r requirements.txt

4️⃣ Add Google API Key

Create a .env file in the root folder and add your Google API key:
GOOGLE_API_KEY=your_google_api_key_here

📖 Usage

Upload a PDF file from the sidebar.

Type a question about the document.

The app retrieves relevant chunks using FAISS.

An LLM (Gemini) generates the final answer.

📌 Tech Stack

Python 3.9+

Streamlit

LangChain

FAISS

Google Generative AI (Gemini)

PyPDF2
