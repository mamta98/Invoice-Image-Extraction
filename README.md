#  Invoice Image Extraction

This project uses **OpenAI's GPT-4o** multimodal model to extract structured key-value pairs from invoice images, such as invoice number, invoice date, and detailed line items. 
It’s designed to be simple, scalable, and completely free of traditional OCR.

---

##  Features

-  Extracts:
  - Invoice Number
  - Invoice Date
  - Line Items (description, quantity, unit price, total)
-  Supports batch processing of `.jpg` images
-  Powered by OpenAI GPT-4o (image + text understanding)
-  Saves results in structured JSON format

---

##  How It Works

1. Reads `.jpg` invoice images from a folder.
2. Converts images to base64 and sends them to GPT-4o via OpenAI's API.
3. GPT-4o returns structured data using natural language and visual understanding.
4. Data is stored in a JSON file (`invoice_extractions.json`).

---

##  Dataset

Images were sourced from this public dataset:

**High-Quality Invoice Images for OCR**  
 https://www.kaggle.com/datasets/osamahosamabdellatif/high-quality-invoice-images-for-ocr/data  
 License: Educational and research use

---

## Folder Structure

invoice-extraction/
├── extract.py # Main script for batch processing
├── invoice_extractions.json # Output file with extracted data
├── /Data # Folder containing invoice images (.jpg)
└── README.md # This file


