# Property Data Scraping & API Automation System

## Overview

This project is a scalable Property Data Scraping & API Automation System developed to extract real estate data dynamically from multiple property websites based on user-defined filters.

The system consists of **15 custom web scrapers** integrated with a **FastAPI backend**, allowing users to request only the data they need through API endpoints. Instead of scraping complete websites, the platform performs targeted data extraction, improving both performance and efficiency.

---

## Features

* 15 Custom Property Website Scrapers
* Dynamic Filter-Based Data Extraction
* FastAPI-Powered Backend
* Pydantic Request Validation
* Automated Scraper Selection
* Structured JSON Responses
* Scalable Architecture
* Efficient Resource Utilization

---

## Workflow

```text
User Filters
      ↓
FastAPI API Request
      ↓
Pydantic Validation
      ↓
Source-Based Scraper Selection
      ↓
Targeted Data Scraping
      ↓
Structured JSON Response
```

---

## Supported Filters

Depending on the selected property source, users can apply filters such as:

* Location
* Property Type
* Price Range
* Bedrooms
* Bathrooms
* Area Size
* Listing Type
* Additional Source-Specific Filters

---

## Technology Stack

### Backend

* Python
* FastAPI
* Pydantic

### Data Extraction

* Custom Web Scrapers
* HTTP Requests
* HTML Parsing

### Data Processing

* JSON Serialization
* Data Validation
* API Response Formatting

---

## API Flow

1. User sends filter parameters through API.
2. FastAPI receives the request.
3. Pydantic validates incoming data.
4. System identifies the target property source.
5. Relevant scraper is executed.
6. Data is extracted according to provided filters.
7. Clean and structured JSON response is returned.

---

## Example Request

```json
{
  "source": "property_website",
  "location": "New York",
  "property_type": "Apartment",
  "min_price": 100000,
  "max_price": 500000
}
```

---

## Example Response

```json
{
  "status": "success",
  "results": [
    {
      "title": "Luxury Apartment",
      "location": "New York",
      "price": "$350,000",
      "property_type": "Apartment"
    }
  ]
}
```

---

## Project Highlights

* Built 15 independent scrapers for different property websites.
* Implemented dynamic filter-based extraction.
* Designed scalable API architecture using FastAPI.
* Reduced unnecessary scraping by extracting only requested data.
* Delivered structured and reusable JSON responses.
* Created a maintainable and extensible scraping framework.

---

## Use Cases

* Real Estate Data Aggregation
* Property Search Platforms
* Market Analysis
* Lead Generation
* Data Collection & Automation
* Business Intelligence Applications

---

## Disclaimer

This project is intended for educational, research, and authorized data collection purposes only. Users are responsible for complying with the terms of service and legal requirements of target websites.

---

## Author

Developed using Python, FastAPI, Pydantic, and Custom Web Scraping Solutions.
