# Facebook_Scraper


## Overview

Welcome to our Facebook Scraper! This powerful tool is designed to extract data from public Facebook pages and groups. It's based on [this project](https://github.com/shaikhsajid1111/facebook_page_scraper), with significant modifications for improved results. We provided also a jupyter notebook that you can use directly to your work.
**NOTE: YOU HAVE TO CHANGE THE PATHS IN THE SCRAPER.PY AND IN THE JUPYTER NOTEBOOK TO YOURS !!!!**

## Features

The scraper generates CSV files with the following fields:

**- `id`**
**- `name`**
**- `shares`**
**- `comments`**
**- `content`**
**- `posted_on`**
**- `image`**
**- `post_url`**
**- `image_content`**

## Special Focus

We've dedicated special attention to the `image_content` field. Recognizing that captions often lack crucial information and a substantial portion of Facebook posts consists of images, we implemented a solution to extract text from photo posts.

## Text Extraction

For text extraction, use the `pytesseract` library along with the `PIL` (Pillow) library. Make sure you have both libraries installed:

```bash
pip install pytesseract Pillow
```
## Tesseract OCR Setup

1-Install Tesseract OCR on your machine. Download it from the official GitHub repository : https://github.com/tesseract-ocr/tessdata
2-Run the following commands in your terminal to install Tesseract OCR (for macOS):

```bash
brew update
brew install tesseract
```
3-Download the Arabic-trained data file (ara.traineddata) from the Tesseract tessdata repository or directly using this link : https://github.com/tesseract-ocr/tessdata/blob/main/ara.traineddata
4-Save the file locally.
```
sudo cp /path/to/ara.traineddata /usr/local/share/tessdata/
```
**(Note: Adjust the path accordingly if Tesseract is installed in a different location.)**

5-Verify the installation by checking for ara.traineddata among other language files:
```
ls /usr/local/share/tessdata/
```
6-Repeat the same process for the English training data.

# Happy scraping! 🚀
