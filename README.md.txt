# 🛠️ Industrial Suppliers Scraper

## 📌 Description
This project is an **intelligent web scraping and search application** designed to extract and analyze data from **industrial material suppliers**.  

It combines:  
- **Search Engines** (DuckDuckGo + Serper with fallback logic)  
- **Web Scraping** (Selenium + BeautifulSoup with fallback logic)  
- **AI-Powered Processing** (Multiple free LLMs with fallback logic for structuring, translation, and JSON output)  
- **DOM Tree Parsing** (recursive sub-link exploration with BeautifulSoup to maximize extracted information)  

A **Flask web interface** provides users with a clean UI to interact with the scraper and download structured results.

---

## 🚀 Features
- 🔍 **Dual Search Engines** → Queries executed on **DuckDuckGo**, with automatic fallback to **Serper**  
- 🌐 **Dual Scraping Engines** → Primary scraping via **Selenium** (JavaScript rendering) with fallback to **BeautifulSoup** (faster static parsing)  
- 📊 **Multi-LLM Fallback Pipeline** → Uses **OpenAI, Groq, Together** and other free LLMs:  
  - Structuring unorganized raw text into meaningful fields  
  - Translating extracted supplier/product information  
  - Generating **JSON output** directly from parsed HTML  
- 🌳 **DOM Tree Scraping** → Crawls **sub-links and nested elements** in the supplier page using BeautifulSoup to maximize extracted data  
- 📂 Export results as **CSV or JSON**  
- 🌎 User-friendly **Flask web interface**  

---

## ⚙️ Tech Stack
- **Backend:** Python (Flask)  
- **Search Engines:** DuckDuckGo Search, Serper API  
- **Scraping:** Selenium, BeautifulSoup, fallback logic  
- **Data Handling:** Pandas  
- **AI Integrations:** OpenAI, Groq, Together, tiktoken  
- **Automation:** nest_asyncio, threading, concurrent futures  
- **Browser Driver:** webdriver-manager (ChromeDriver)  

---

📦 Installation

Clone the repository

git clone https://github.com/your-username/industrial-supplier-scraper.git
cd industrial-supplier-scraper


Create a virtual environment (recommended)

python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows


Install dependencies

pip install -r requirements.txt

▶️ Usage

The code is in app.ipynb:

Open Jupyter Notebook:

jupyter notebook


Open app.ipynb in the browser.

Run the notebook cells to execute the scraper and see outputs.

## 🖼️ Screenshots

**Input Page (Accueil):**  
![Input Page](images/input_page1.png)
![Input Page](images/input_page2.png)

**Results Page (Output):**  
![Results Page](images/results_page1.png)
![Results Page](images/results_page2.png)