# 🚀 [Tips Hindawi](https://www.tipshindawi.com/) Challenge (June–July) 2026

> 🏆 This repository is my official submission for the [ **Tips Hindawi** ](https://www.tipshindawi.com/) **Challenge (June–July) 2026**.

## 👤 Participant

| Field            | Value                                |
| ---------------- | ------------------------------------ |
| Full Name        |     Ahmed Soliman Saad Abdelhamid    |
| Project Name     | AI PDF Chat Assistant                |
| GitHub Username  |      ahmedA00-sys                    |
| Challenge Batch  | June–July 2026                       |
| Training Program | Large Language Models (LLMs) Program |

---

# 📖 Project Overview

The **AI PDF Chat Assistant** is a beginner-friendly local application that demonstrates a complete Retrieval-Augmented Generation (RAG) pipeline. It allows users to upload any PDF document and ask questions about its content. The AI retrieves the most relevant sections from the document and generates accurate answers based solely on that context, preventing the model from hallucinating or using outside knowledge.

The project is structured as a series of 10 progressive Jupyter notebooks that walk through each step of the RAG process, from loading and splitting text to creating embeddings, storing them in a vector database, and building a simple web interface with Gradio.

---

# ✨ Features

* **Local Execution:** The entire system runs locally on the user's machine using Ollama and Mistral, ensuring data privacy.
* **Accurate Retrieval:** Uses HuggingFace Embeddings and ChromaDB to find the most relevant document chunks for any query.
* **Hallucination Prevention:** Engineered prompts force the LLM to answer only using the provided context.
* **Structured Output:** Utilizes Pydantic to parse the LLM's response into a structured format containing the answer, source page, confidence level, and retrieved context.
* **User-Friendly Interface:** Features a simple web GUI built with Gradio for uploading PDFs and asking questions.

---

# 🛠️ Technologies Used

* **Programming Language:** Python 3.9+
* **Environment:** Jupyter Notebooks (.ipynb)
* **LLM Framework:** LangChain
* **Local LLM Execution:** Ollama
* **Language Model:** Mistral
* **Embeddings:** HuggingFace (`sentence-transformers/all-MiniLM-L6-v2`)
* **Vector Database:** ChromaDB
* **UI Framework:** Gradio
* **Data Parsing:** Pydantic Output Parser

---

# ⚙️ Installation

To run this project locally, you need to install Ollama and set up the Python environment.

1. **Install Ollama:**
   Download and install Ollama from [ollama.com](https://ollama.com/).

2. **Start Ollama and Pull the Model:**
   Open a terminal and run:
   ```bash
   ollama serve
   ollama pull mistral
   ```

3. **Create and Activate a Virtual Environment:**
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

4. **Install Python Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

5. **Prepare Sample Data:**
   Place any PDF file you want to analyze into the `data/` folder and name it `sample.pdf`.

---

# 🚀 Usage

The project is designed to be run sequentially through the Jupyter notebooks.

1. **Start Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

2. **Run Notebooks in Order:**
   * `01_Installation.ipynb`: Verify your setup.
   * `02_Load_PDF.ipynb` to `05_ChromaDB.ipynb`: Learn how to load, split, embed, and store document data.
   * `06_RAG.ipynb`: Build the core RAG pipeline.
   * `07_Prompt_Engineering.ipynb` & `08_Output_Parser.ipynb`: Improve prompts and structure the output.
   * `10_Final_Project.ipynb`: Run the complete application.

3. **Launch the GUI:**
   After running the cells in `10_Final_Project.ipynb`, open your web browser and navigate to `http://localhost:7860` to use the Gradio interface. Upload a PDF and ask questions.

---

# 📸 Demo

*Add screenshots, GIFs, or a demo video.*
*(Screenshots of the Gradio interface showing a PDF upload and the AI's structured response can be added here.)*

---

# 📈 Results

The project successfully implements a full RAG pipeline that can process PDF documents of various sizes, accurately retrieve relevant context, and generate structured, factual answers without hallucinations. The use of local models via Ollama ensures the solution is cost-effective and private.

---

# 🔮 Future Improvements

* Implement chat history to allow for multi-turn conversations about the document.
* Add support for multiple concurrent PDF uploads and cross-document querying.
* Integrate a GPU-accelerated setup for faster embedding and inference times.
* Replace the simple Gradio interface with a more robust web application using a frontend framework.

---

# 📚 About the Challenge

This project was developed as part of the [**Tips Hindawi**](https://www.tipshindawi.com/) **Challenge (June–July) 2026**.

[Tips Hindawi](https://www.tipshindawi.com/) is the internships department of [**Edrak for Ai**](https://edrak4ai.com/en), and the challenge encourages participants to build real-world projects, apply practical skills, and showcase their work through GitHub.

For more information about the challenge, training programs, and upcoming batches, visit the official [Tips Hindawi](https://www.tipshindawi.com/) website.

---

# 📄 License

This project is shared for educational and portfolio purposes.
