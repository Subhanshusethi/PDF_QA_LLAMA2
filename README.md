---

# 📄 PDF_QA_Llama3.2

**PDF_QA_Llama3.2** is an AI-powered PDF question-answering application built using **LangChain**, **FAISS**, **Sentence-Transformers**, and **Meta’s Llama 3.2** (quantized). It allows users to upload PDF documents, extract their content, and ask questions — receiving intelligent, context-aware answers in real time.

---

## 🚀 Features

- 📥 Upload any PDF file  
- 🔍 Automatic content extraction  
- 💬 Ask questions in natural language  
- 🧠 Powered by HuggingFace + LangChain + FAISS  
- ⚡ Uses quantized **Llama 3.2** model for fast inference  
- 🧾 Retrieves the most relevant chunks from your PDF for accurate answering  
- 🖥️ Easy-to-use **Streamlit interface**  

---

## 🛠️ Tech Stack

- `Transformers` (HuggingFace)
- `Llama 3.2` via 4-bit quantized loading (BitsAndBytes)
- `LangChain` (ConversationalRetrievalChain)
- `FAISS` (Vector store for semantic search)
- `SentenceTransformers` (`all-mpnet-base-v2`)
- `Streamlit` (Frontend)
- `PyPDFLoader` (Document ingestion)

---

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/your-username/PDF_QA_Llama3.2.git
cd PDF_QA_Llama3.2

# Install dependencies
pip install -r requirements.txt
```

---

## ⚙️ Usage

1. **Add your model**:  
   Replace `"ADD YOUR HF TOKEN"` in the code with your HuggingFace model ID or local path to the quantized Llama 3.2 model.

2. **Run the app**:

```bash
streamlit run app.py
```

3. **Upload a PDF** and start asking questions!

---

## 📸 Demo

Coming soon!

---

## 📁 Directory Structure

```
.
├── app.py                  # Main Streamlit app
├── README.md               # Project documentation
├── requirements.txt        # Required Python packages
```

---

## 📚 Example Models

- LLM: [`meta-llama/Llama-3-8b`](https://huggingface.co/meta-llama) (use quantized 4-bit versions for faster inference)
- Embeddings: `sentence-transformers/all-mpnet-base-v2`

---

## 🧠 Behind the Scenes

- **PDF Ingestion** → `PyPDFLoader`
- **Chunking** → `RecursiveCharacterTextSplitter`
- **Embeddings** → `HuggingFaceEmbeddings`
- **Vector Store** → `FAISS`
- **Answering** → `ConversationalRetrievalChain` with LLM pipeline

---

## 📄 License

This project is licensed under the MIT License. See `LICENSE` for details.

---

## 🙌 Acknowledgements

- [Meta AI](https://ai.meta.com/) for Llama 3
- [HuggingFace](https://huggingface.co/)
- [LangChain](https://www.langchain.com/)
- [FAISS](https://github.com/facebookresearch/faiss)

---

Would you like a custom logo/banner for your repo too?
