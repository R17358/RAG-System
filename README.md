# RAG Q&A App

## Overview
The **RAG Q&A App** is a Retrieval-Augmented Generation (RAG) system that allows users to ask questions based on provided documents, links, or text. The app retrieves relevant information using FAISS vector stores and generates answers using Google's Gemini API.

## Features
- Supports multiple input types: **Text, PDF, DOCX, TXT, and Links**.
- Uses **FAISS** for efficient similarity search.
- Embeds text using **HuggingFace sentence-transformers**.
- Generates answers using **Google Gemini API**.
- Interactive Streamlit UI for a seamless user experience.

## Technologies Used
- **FastAPI**
- **Streamlit**
- **FAISS**
- **HuggingFace Embeddings**
- **Google Gemini API**
- **PyPDF2** (for PDF processing)
- **python-docx** (for DOCX processing)
- **LangChain** (for text processing and retrieval)

## Installation
### Prerequisites
Ensure you have Python installed (>= 3.8). Install dependencies:
```sh
pip install fastapi streamlit faiss-cpu langchain langchain-community langchain-huggingface PyPDF2 python-docx google-generativeai dotenv
```

### Environment Setup
Create a `.env` file and add your **Google Gemini API Key**:
```
GEMINI_API_KEY=your_api_key_here
```

## Usage
### Running the App
```sh
streamlit run app.py
```

### How to Use
1. Select an **Input Type** (Text, PDF, DOCX, TXT, or Link).
2. Upload files or enter a link/text.
3. Click **Proceed** to process the input.
4. Enter your question in the text box.
5. Click **Submit** to generate an answer.

## Project Structure
```
📂 project_root
│-- app.py                  # Main Streamlit app
│-- .env                    # API key configuration
│-- requirements.txt        # Required dependencies
```

## Acknowledgments
- **Hugging Face** for embeddings.
- **Google Gemini API** for text generation.
- **FAISS** for efficient document retrieval.

## Future Enhancements
- Implement caching for faster response times.
- Support additional document formats.
- Deploy as a web service using **FastAPI**.

## License
This project is licensed under the MIT License.

