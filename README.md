# 📄 PDF Query System with LangChain

An intelligent document querying system that allows users to ask questions about PDF documents using natural language. Built with LangChain, OpenAI, and FAISS for semantic search and retrieval.

## 🌟 Features

- **PDF Text Extraction**: Automatically extracts and processes text from PDF documents
- **Semantic Search**: Uses OpenAI embeddings and FAISS for intelligent document retrieval
- **Natural Language Q&A**: Ask questions in plain English and get accurate answers
- **Context-Aware Responses**: Retrieves relevant document sections to generate informed answers
- **Fast Vector Search**: Efficient similarity search using FAISS vector database

## 🛠️ Technologies Used

- **LangChain**: Framework for building LLM applications
- **OpenAI GPT-3.5/4**: Language model for question answering
- **FAISS**: Vector database for semantic search
- **PyPDF2**: PDF text extraction
- **Python 3.12**: Core programming language

## 📋 Prerequisites

- Python 3.8+
- OpenAI API key

## 🚀 Installation

1. **Clone the repository**
```bash
git clone https://github.com/KrishnaSaiKoduru/Query_Document_langchain.git
cd Query_Document_langchain
```

2. **Create a virtual environment**
```bash
python -m venv venv
```

3. **Activate the virtual environment**
```bash
# Windows
venv\Scripts\activate

# Mac/Linux
source venv/bin/activate
```

4. **Install dependencies**
```bash
pip install -r requirements.txt
```

## ⚙️ Configuration

1. **Create a `.env` file** in the project root:
```env
OPENAI_API_KEY=your-openai-api-key-here
```

2. **Get your OpenAI API key** from [OpenAI Platform](https://platform.openai.com/api-keys)

## 📖 Usage

### Running the Jupyter Notebook

1. **Start Jupyter Notebook**
```bash
jupyter notebook
```

2. **Open** `document_query_langchain.ipynb`

3. **Run the cells** sequentially to:
   - Load and process your PDF
   - Create vector embeddings
   - Ask questions about the document

### Example Usage
```python
# Load your PDF
pdf_path = "path/to/your/document.pdf"

# Ask questions
query = "What is this document about?"
answer = ask_question(query)
print(answer)
```

### Sample Questions
```python
# Summarization
"What are the main topics covered in this document?"

# Specific information
"What does the document say about [topic]?"

# Details
"Explain [specific concept] mentioned in the document"
```

## 📁 Project Structure
```
Query_Document_langchain/
│
├── document_query_langchain.ipynb  # Main Jupyter notebook
├── .env                             # Environment variables (not tracked)
├── .gitignore                       # Git ignore file
├── requirements.txt                 # Python dependencies
├── README.md                        # Project documentation
└── Magazine.pdf                     # Sample PDF (your document)
```

## 🔧 How It Works

1. **PDF Processing**: Extracts text from PDF using PyPDF2
2. **Text Chunking**: Splits text into manageable chunks with overlap
3. **Embedding Generation**: Creates vector embeddings using OpenAI
4. **Vector Storage**: Stores embeddings in FAISS for fast retrieval
5. **Query Processing**: Converts questions to embeddings
6. **Similarity Search**: Finds most relevant document chunks
7. **Answer Generation**: Uses GPT to generate answers from context

## 📦 Dependencies
```txt
langchain
langchain-openai
langchain-community
langchain-text-splitters
PyPDF2
faiss-cpu
tiktoken
python-dotenv
openai
```

## 👤 Author

**Krishna Sai Koduru**
- GitHub: [@KrishnaSaiKoduru](https://github.com/KrishnaSaiKoduru)


⭐ If you find this project useful, please consider giving it a star!
