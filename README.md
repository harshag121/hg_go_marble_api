# GoMarble Reviews API

## Overview

This API server extracts reviews from any product page using browser automation (Playwright) and dynamic CSS selector detection powered by OpenAI’s API. The endpoint `/api/reviews?page={url}` returns the count and details of reviews in a standardized JSON format.

## Features

- **Dynamic CSS Identification:** Uses OpenAI to analyze an HTML snippet and provide CSS selectors.
- **Pagination Handling:** Automatically navigates through paginated reviews.
- **Modern Stack:** Built with FastAPI, Playwright, and OpenAI’s API.

## Prerequisites

- **Python 3.8+**
- **Node.js (for Playwright browser installation)**
- An **OpenAI API key**

## Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/harshag121/go_marble_api.git
   cd go_marble_api

2. ### For env setup and dependiencies for project
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt

3. ### For installing Browser
playwright install

4. Create a .env file and add this in that 

OPENAI_API_KEY=your_openai_api_key_here
