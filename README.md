# Multimodal-RAG-application
<img width="660" alt="Screenshot 2024-09-20 at 6 45 11 PM" src="https://github.com/user-attachments/assets/a0a892c4-f633-47fb-bbe1-801679a82daa">


The goal was to create the above represented Multimodal RAG Application without using an OCR 
This project implements a **Multimodal Retrieval-Augmented Generation (RAG)** system that extracts text and images from PDF documents, generates responses to user queries using text and image retrieval, and then summarizes the response. The system uses **CLIP**, **BLIP**, and **T5** models for embeddings, answer generation, and summarization, respectively.

## Key Features

- **PDF Text and Image Extraction**: Extracts both text and images from uploaded PDF documents.
- **Multimodal Embedding**: Uses **CLIP** to generate embeddings for both text and images.
- **Text Chunking**: Automatically splits long text into chunks for efficient processing.
- **Faiss Indexing**: Efficiently stores and retrieves embeddings using **Faiss** for similarity search.
- **Answer Generation**: Uses **BLIP** to generate multimodal answers based on text and images.
- **Summarization**: Summarizes the generated answer using the **T5 model** for a concise and readable response.
- **Automated Feedback Loop**: Evaluates the quality of generated responses based on length and repetition, logging the feedback.

## Models Used

- **CLIP**: For text and image embeddings.
- **BLIP**: For generating answers from multimodal input (text and images).
- **T5**: For abstractive summarization of generated answers.

## Getting Started

### Prerequisites

1. **Python** (3.8 or higher)
2. **Google Colab** (if running the notebook in Colab)
3. **Python Libraries**:
   - `transformers`
   - `torch`
   - `faiss`
   - `fitz` (PyMuPDF)
   - `PIL` (Pillow)
   - `pandas`
   - `matplotlib`

To install the required libraries, run:

```bash
pip install transformers torch faiss-cpu pymupdf Pillow pandas matplotlib
