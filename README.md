# pdf-analyser-chatbot

PDF Chatbot
This project allows you to chat with the contents of PDF documents. It uses Streamlit for the web interface, PyPDF2 for PDF reading, LangChain for text splitting and embedding, and Google Generative AI for answering questions based on the PDF content.

Features
PDF Upload and Processing: Upload multiple PDF files, which are then processed to extract text.
Text Chunking: The extracted text is split into manageable chunks for better performance.
Vector Store Creation: A vector store is created using embeddings to facilitate quick similarity searches.
Conversational Interface: Ask questions related to the PDF content, and receive detailed answers based on the processed text.
Installation:
streamlit
langchain
google-generativeai
python-dotenv
langchain-community
langchain-google-genai
PyPDF2

Code Explanation
PDF Extraction (get_pdf_text): Reads and extracts text from the uploaded PDF files.
Text Chunking (get_text_chunks): Splits the extracted text into chunks for better processing.
Vector Store Creation (get_vector_store): Creates and saves a vector store using FAISS and Google Generative AI embeddings.
Conversational Chain (get_conversational_chain): Defines the prompt template and loads the QA chain for generating answers.
User Input Handling (user_input): Handles user questions, performs similarity search, and provides answers.
Main Application (main): Sets up the Streamlit app, handles file uploads, and processes user input.
Troubleshooting
API Key Issues: Ensure your Google API key is valid and properly set in the .env file.
Dependency Errors: Verify that all dependencies are installed correctly. Use pip to install any missing packages.
