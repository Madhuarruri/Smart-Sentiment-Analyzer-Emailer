SMART SENTIMENT ANALYZER & EMAILER

Smart Sentiment Analyzer & Emailer is a complete web application that combines Amazon web scraping, NLP-based sentiment analysis, an intelligent chatbot interface, and an email alert system. It allows users to paste an Amazon product URL, chat with a smart assistant to explore product reviews, and receive email notifications when the price drops below a set threshold.

Project Highlights

AI Chatbot Interface – A smart assistant that helps users interactively analyze product reviews

Amazon Review Scraper – Dynamically fetches reviews from any product URL on Amazon

Sentiment Analysis – Uses TextBlob to classify reviews as Positive, Negative, or Neutral

Visual Dashboard – Displays review stats and pie chart representation of sentiments

Email Notifications – Sends alerts when a product’s price drops below user-defined limits
SCREEN SHOTS:
![image](https://github.com/user-attachments/assets/235a9ce9-7ff6-46ca-a64e-fd4a9172cde8)
![image](https://github.com/user-attachments/assets/29fdc0b1-5650-43ea-81f1-28dd31c512f4)
![image](https://github.com/user-attachments/assets/c5a5b88a-c418-4302-a62f-2a0f450bf108)

Tech Stack

Frontend: HTML, CSS, JavaScript
Backend: Python, Flask
Libraries Used: BeautifulSoup, Requests, TextBlob, smtplib, Matplotlib
Deployment: Render (cloud-based hosting platform)

Folder Structure

AMAZON_PT/
|-- app.py → Main Flask application
|-- reviews_generator.py → Review scraper and sentiment analyzer
|-- chatbot.py → Chatbot logic and smart interactions
|-- requirements.txt → Python dependencies
|-- Procfile → Deployment configuration for Render
|-- README.md → Project documentation
|-- templates/ → HTML templates (index.html, result.html)
|-- static/ → CSS, images, JS (style.css, rev.png)

How to Run Locally

Clone the project using Git
git clone https://github.com/YOUR_USERNAME/smart-sentiment-analyzer-emailer.git
cd smart-sentiment-analyzer-emailer

Install required dependencies
pip install -r requirements.txt

Run the Flask application
python app.py

Open your browser and go to
http://127.0.0.1:5000/

How to Deploy on Render

Push the code to your GitHub repository

Go to https://render.com and create a new Web Service

Connect your GitHub repo

Set:
Build command: pip install -r requirements.txt
Start command: gunicorn app:app

Add Environment Variables:
EMAIL_USER = your Gmail address
EMAIL_PASS = your Gmail app password

Click Deploy and access your live app

Gmail Setup for Email Notifications

Use Gmail App Passwords (ensure 2-factor authentication is enabled)

Add EMAIL_USER and EMAIL_PASS in Render's environment settings securely

These credentials are used in Python to send emails via smtplib

Future Scope

Add an AI-based review summarizer

Detect and highlight fake or bot reviews

Enable scraping for other platforms like Flipkart or Snapdeal

Add a background scheduler to periodically track and compare prices

Author

Madhu Arruri
JNTUH UCESTH Hyderabad
Graduation Year: 2026
Contact: madhu@email.com

Like This Project?

If you found this useful, give it a star on GitHub and share it with others preparing smart sentiment-based applications!
