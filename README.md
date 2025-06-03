# cafef-crawler
Crawl financial news from CafeF, analyze promotional articles using Gemini AI, and extract structured insights to Google Sheets.

# CafeF Competitor Program Analyzer

This project automates the process of collecting and analyzing financial news articles from CafeF.vn, with a focus on detecting promotional campaigns from competing stock brokerages (e.g., VPS, SSI, DNSE, TCBS).

## Overview

- Crawl news articles from CafeF using Selenium in Google Colab
- Extract full article content and publication time
- Detect mentions of competitor firms using keyword-based filtering
- Use Gemini Flash API to:
  - Classify article type (product PR, brand PR, or neutral)
  - Extract campaign details: name, offer, conditions, target customers
- Match detected programs with internal MBS database from Google Sheets
- Save results to Google Sheets and export to Excel

## Technologies

- Python 3.10
- Selenium (Web crawling)
- Google Colab
- Gemini Flash API (Google Generative AI)
- Google Sheets API (`gspread`)
- Pandas, OpenPyXL

## Repository Structure

cafef-analyzer/
│
├── cafef_pipeline.ipynb # Main Google Colab notebook
├── requirements.txt # List of required packages
├── README.md # This documentation
├── sample_output.xlsx # Optional: sample result
└── assets/
└── screenshot.png # Optional: output preview


## How to Run

1. Open `cafef_pipeline.ipynb` in Google Colab  
2. Provide your Gemini API Key and Google Service Account JSON  
3. Configure the Google Sheet URL and worksheet names  
4. Run all cells to:
   - Crawl articles
   - Analyze content via Gemini
   - Save structured data to Google Sheets and Excel

## Example Output

The system outputs a structured dataset including:
- Article title, time, URL
- Competitor focus
- Campaign name and offer
- AI-generated summary and extracted fields
- Matching result with MBS’s program database

## Contact

Developed by Hoàng Thị Mai Phương 
For collaboration or questions, please contact: hmphuonggg32@gmail.com
