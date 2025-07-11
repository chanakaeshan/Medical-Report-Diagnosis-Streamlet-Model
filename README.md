# Medical Report Diagnosis Streamlet Chat App.

### Overview
This Streamlit application is designed to assist in the analysis and diagnosis of medical reports, specifically pathology laboratory blood test reports. The app allows users to upload medical reports in either JPG/JPEG or PDF formats. Once uploaded, the application extracts text from the report, summarises it using a powerful language model, and provides an interface for users to ask specific questions about the report's content.

## Features
- **File Upload**: Supports uploading medical reports in JPG, JPEG, and PDF formats.
- **Text Extraction**:
  - For JPG/JPEG files: Optical Character Recognition (OCR) is performed using easyocr to extract text from the images.
  - For PDF files: Text is directly extracted using PyMuPDF.
- **Text Summarisation**: Utilises the meta-llama/Meta-Llama-3-8B-Instruct language model from Hugging Face to generate concise summaries of the extracted text.
- **Question-Answer Interface**: Enables users to interact with the summarised report by posing specific questions. The app uses a FAISS vector store to retrieve relevant information from the text and provide accurate answers.


## Installation
1. **Clone the repository**:
```
https://github.com/chanakaeshan/Medical-Report-Diagnosis-Streamlet-Model.git

cd Medical-Report-Diagnosis-Streamlet-Model.git
```
3.  **Install the required packages**:
```pip install -r requirements.txt```

4.  **Run the Streamlit app**:
```streamlit run src/report.py```

## Dependencies
- **Streamlit**: For building the web interface.
- **easyocr**: For OCR processing of images.
- **PyMuPDF**: For text extraction from PDF files.
- **LangChain**: For text splitting and summarisation.
- **FAISS**: For vector-based information retrieval.
- **Hugging Face**: For accessing the language models.


## Usage
- Upload a Report: Drag and drop a medical report in JPG, JPEG, or PDF format.
- Generate Summary: Click on "Summarise Report" in the sidebar to generate a concise summary of the report.
- Ask Questions: Use the chat interface to ask specific questions about the report's content.








Medical Report Diagnosis Streamlet Model
