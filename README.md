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

1. Clone the repository:
   ```bash
   git clone https://github.com/harshag121/hg_go_marble_api.git
   cd hg_go_marble_api
   ```

2. Set up a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Install Playwright browsers:
   ```bash
   playwright install
   ```

4. Configure environment variables:
   Create a `.env` file in the root directory and add the following line:
   ```env
   OPENAI_API_KEY=your_openai_api_key_here
   ```
   Replace `your_openai_api_key_here` with your actual OpenAI API key.
