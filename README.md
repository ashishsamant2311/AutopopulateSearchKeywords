# Automated Keyword Extraction for E-Commerce Products 🚀

## Overview

In the ever-expanding world of e-commerce, effective search keyword assignment is essential to ensure products are discoverable by customers. However, the process of curating search keywords often faces significant challenges:

### Challenges
1. **Manual Effort**: 
   - Assigning keywords requires extensive manual work by cataloging teams or sellers.
2. **Spelling Errors**: 
   - Misspelled keywords may not match customer search queries, leading to reduced discoverability.
3. **Keyword Stuffing**: 
   - Sellers may misuse irrelevant yet popular keywords to boost product visibility artificially.

To address these issues, we utilized the **Mistralai/Mistral-7B-Instruct-v0.2** model—a cutting-edge, instruction-fine-tuned Large Language Model (LLM)—to automate and optimize keyword generation for e-commerce products.

---

## Approach

### Why Mistral-7B-Instruct?
- **Instruction-Fine-Tuned**: This LLM is optimized for language generation tasks, making it ideal for producing accurate and relevant keywords.
- **Large Context Window**: With a context window of 32K characters, the model efficiently handles extensive product descriptions and features, ensuring comprehensive keyword coverage.

### Quantization for Efficiency
Due to operational infrastructure constraints, we employed **BitsAndBytes** quantization to reduce the model size:
- **4-Bit Quantization**: Enabled the model to operate with just 5GB of memory.
- **Deployment**: Successfully loaded and inferred using a Google Colab T4 GPU.

---

## Dataset
The dataset used for this project consists of product details from **Flipkart**, including titles, descriptions, and key features. This ensures that the generated keywords are relevant to the e-commerce domain.

---

## Benefits of Our Solution
1. **Reduced Manual Effort**: Automated keyword generation streamlines the process, saving time for cataloging teams and sellers.
2. **Improved Accuracy**: Eliminates the possibility of spelling errors and ensures high-quality, search-relevant keywords.
3. **Minimized Keyword Stuffing**: Generates contextually appropriate keywords, reducing instances of irrelevant or spammy keyword usage.

---

## How It Works
- **Input**: Product title, description, and features.
- **Processing**: The model sifts through the input text, leveraging its extensive language understanding capabilities to produce optimal keywords.
- **Output**: A list of high-quality, search-relevant keywords.

---

## Project Contents
- **Notebook**: Detailed implementation in `KeywordextractionLLM.ipynb`.
- **Dataset**: Flipkart product catalog.
- **Models Used**: 
  - Mistralai/Mistral-7B-Instruct-v0.2
  - Quantized version using BitsAndBytes.
- **Tools**: Google Colab with T4 GPU for model inference.

---

## Getting Started

### Prerequisites
- Google Colab account.
- Python environment with the following libraries installed:
  - `transformers`
  - `bitsandbytes`
  - `torch`

### Steps to Run
1. Clone this repository.
2. Open `KeywordextractionLLM.ipynb` in Google Colab.
3. Follow the instructions in the notebook to load the quantized model and generate keywords.

---

## Future Enhancements
- Fine-tuning the model further for domain-specific keyword generation.
- Exploring multi-language support for a global e-commerce audience.
- Optimizing inference speed for real-time applications.

---

## Contributing
I welcome contributions to improve this
