# Image Scraping Web Application

This is a Python web application built with Flask that allows users to search for images on Google and download them. The downloaded images are saved to a specified directory, and the image data is stored in a MongoDB database.

## Features

- Search for images on Google based on user input.
- Download and save the images to a specified directory.
- Store image data in a MongoDB database.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.x installed on your system.
- Required Python libraries: Flask, Flask-CORS, requests, BeautifulSoup4, pymongo.

## Setup and Usage

1. Clone or download this repository to your local machine.

2. Navigate to the project directory.

3. Install the required Python libraries using pip:

   ```bash
   pip install -r requirements.txt
   ```

4. Run the application:

   ```bash
   python app.py
   ```

   The application will start and be accessible at `http://localhost:8000/` in your web browser.

5. Use the web interface to input search queries and download images from Google.

## Configuration

You need to configure the MongoDB connection in the `app.py` file. Update the following line with your MongoDB connection string:

```python
client = pymongo.MongoClient("mongodb+srv://username:password@cluster.mongodb.net/?retryWrites=true&w=majority")
```

Replace `username`, `password`, and `cluster.mongodb.net` with your MongoDB credentials.

## Logging

The application logs any errors or exceptions to a `scrapper.log` file located in the project directory.

---
