# AI Research Assistant  

An AI-powered research assistant for exploring academic papers from **arXiv**. This tool simplifies the process of fetching, analyzing, and answering questions based on academic papers using advanced AI technologies like **LangChain**, **Qdrant**, and **Ollama**. It features a user-friendly web interface built with **Gradio**.  

## Features  
- **Arxiv Integration**: Automatically fetches academic papers based on a user-specified topic.  
- **PDF Processing**: Extracts content from PDFs and organizes it into manageable chunks.  
- **Qdrant Vector Store**: Stores and retrieves embeddings of paper content for efficient search and analysis.  
- **AI-Powered Responses**: Uses **Ollama** to generate answers based on the paper content.  
- **Interactive Interface**: Provides a simple, intuitive interface via **Gradio**.  

## How It Works  
1. Enter a research topic and a question in the Gradio interface.  
2. The assistant fetches relevant papers from **arXiv**.  
3. It processes the papers into text chunks, stores them in **Qdrant**, and uses **Ollama** to generate intelligent answers.  

### Example Usage  
- **Topic:** "Voice Cloning"  
- **Question:** "How is the Transformer model used in voice cloning?"  
- **Output:** A detailed response derived from the processed academic papers.  

## Installation  

### Step 1: Install Dependencies  
Run the following command to install the required Python libraries:  
```bash  
pip install gradio arxiv langchain_community qdrant-client PyPDF2 langchain
```
### Step 2: Install Ollama
- Download Ollama from its official website.
- Pull the Llama 2 (7B) model using:
```bash
ollama pull llama2:7b-chat  
```
**Optional**: Install CUDA for GPU acceleration if you're using large models.

## Running the Application
1. Clone this repository:
```bash
git clone https://github.com/your-username/ai-research-assistant.git  
cd ai-research-assistant  
```
2. Install all dependencies as described above.
3. Run the application:
```bash
python app.py  
```
4. Open the Gradio interface in your browser (usually at http://127.0.0.1:7860).
## Components
- ### Gradio: Provides the web-based user interface.
- ### Arxiv API: Fetches relevant academic papers.
- ### LangChain: Processes text and handles NLP tasks.
- ### Qdrant: Stores and retrieves embeddings of paper content.
- ### Ollama: Generates intelligent, conversational responses.

  
## Code Highlights

### Paper Processing
The assistant uses a core function to manage the process:

- Downloads papers from arXiv.
- Extracts and splits content into manageable chunks.
- Stores embeddings in Qdrant for efficient search.
  
### Interactive Gradio UI

- The interface allows users to:
- Input a research topic and a specific question.
- View AI-generated answers based on the processed paper content.


## Example Input and Output

### Input:
- Topic: "Voice Cloning"
- Question: "How is the Transformer model used in voice cloning?"
  
### Output:
A concise, AI-generated explanation based on the academic papers retrieved and processed.


## Future Improvements
- Add support for more AI models and vector stores.
- Expand document sources beyond arXiv.
- Include advanced features like sentiment analysis or conversation summarization.

  



