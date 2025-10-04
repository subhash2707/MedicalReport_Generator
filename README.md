# 📝 AI-powered medical report summarizer

Efficiently condense lengthy reports and documents using advanced AI and OCR technologies.

![Version](https://img.shields.io/badge/version-1.0.0-blue) ![License](https://img.shields.io/badge/license-None-red) ![Stars](https://img.shields.io/github/stars/subhash2707/MedicalReport_Generator?style=social) ![Forks](https://img.shields.io/github/forks/subhash2707/MedicalReport_Generator?style=social)

## ✨ Features

* 📄 **Document OCR**: Accurately extract text from various document formats (e.g., PDFs, images) using Tesseract.js.
* 🧠 **Intelligent Summarization**: Generate concise and coherent summaries of reports, focusing on key information.
* ⚡ **Fast Processing**: Optimized backend for efficient handling and summarization of large documents.
* ⚙️ **Scalable API**: Robust and well-structured API built with Express.js, ready for integration into other applications.
* 🔍 **Text Similarity & Relevance**: Utilizes `fuzzball` and `string-similarity` for enhanced text processing and ensuring summary relevance.

## 🚀 Installation Guide

Follow these steps to set up and run the AI-powered Report Summarizer on your local machine.

### Prerequisites

* Node.js (LTS version recommended)
* npm (comes with Node.js) or Yarn

### Step-by-Step Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/subhash2707/MedicalReport_Generator.git
    cd MedicalReport_Generator
    ```

2. **Install Dependencies**:
    ```bash
    npm install
    # or if you use Yarn
    # yarn install
    ```

3. **Environment Configuration**:
    Create a `.env` file in the root directory of the project. This file will store your environment variables.
    ```
    PORT=3000
    TESSDATA_PREFIX=./
    # Add any other necessary environment variables here
    ```
    * `PORT`: The port on which the server will run.
    * `TESSDATA_PREFIX`: Specifies the directory where Tesseract language data files (`.traineddata`) are located. Ensure `eng.traineddata` is accessible at this path.

4. **Tesseract Language Data**:
    The project includes `eng.traineddata` for English OCR. If you need other languages, you might need to download additional `.traineddata` files from the [Tesseract OCR GitHub](https://github.com/tesseract-ocr/tessdata) and place them in a directory accessible by `TESSDATA_PREFIX`.

## 💡 Usage Examples

Once the server is running, you can interact with the summarization API.

### Starting the Server

To start the backend server, run:

```bash
npm start
# or
node server.js
