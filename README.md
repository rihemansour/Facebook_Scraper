<h1> Facebook Scraper </h1>

[![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https://github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity)
[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-360/)

<p> No need of API key, No limitation on number of requests. Import the library and <b> Just Do It !<b> </p>

## Overview

Welcome to our Facebook Scraper! This powerful tool is designed to extract data from public Facebook pages and groups. It's based on [this project](https://github.com/shaikhsajid1111/facebook_page_scraper), with significant modifications for improved results.
We also provided an exemple of use of this project in a jupyter notebook you can easily copy the code and use it in your work **:)**

**NOTE: You need to change the paths in the scraper.py and the jupyter notebook to yours**

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
1-Install Tesseract OCR on your machine. Download it from the official GitHub repository: https://github.com/tesseract-ocr/tessdata<br>
2-Run the following commands in your terminal to install Tesseract OCR (for macOS):
```
brew update
brew install tesseract
```
3-Download the Arabic-trained data file (ara.traineddata) from the Tesseract tessdata repository or directly using this link: https://github.com/tesseract-ocr/tessdata/blob/main/ara.traineddata<br>
4-Save the downloaded file to your local machine.<br>
5-Copy the file to the tessdata folder using the following commands. Replace /usr/local/share/tessdata/ with the appropriate path on your system if it's different:
```
sudo cp /path/to/ara.traineddata /usr/local/share/tessdata/
```
or
```
sudo mv /path/to/ara.traineddata /usr/local/share/tessdata/
```
6-Verify the installation by checking for the Arabic-trained data file:
```
ls /usr/local/share/tessdata/
```
Repeat the same process for the English training data.<br>

# Happy scraping! 🚀
