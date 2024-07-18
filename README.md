# Stock News Alert System
Before running the script, you need to set up the following:

1. Obtain API keys for Alpha Vantage and News API.
2. Obtain your Twilio Account SID, Auth Token, and a Twilio phone number.
3. Replace placeholders in the script (STOCK_API_KEY, NEWS_API_KEY, TWILIO_SID, TWILIO_AUTH_TOKEN, VIRTUAL_TWILIO_NUMBER, VERIFIED_NUMBER) with your actual credentials.

# Functionality
Step 1: Fetches the daily closing stock prices for the specified company (e.g., TSLA - Tesla Inc) from Alpha Vantage.
Step 2: Calculates the percentage difference between yesterday's closing price and the day before yesterday's closing price.
Step 3: If the percentage difference exceeds a specified threshold (in this case, 1%), it fetches the latest news articles related to the company using the News API.
Step 4: Formats the fetched news articles and sends each article as a separate SMS message using Twilio.

# Resources Used
Alpha Vantage API: Used for retrieving stock market data.
News API: Used for fetching news articles related to the specified company.
Twilio API: Used for sending SMS messages with news alerts.

# Notes
Ensure that you do not expose your API keys and credentials publicly (e.g., by committing them to version control systems).
Adjust the threshold (1% in this case) for significant stock price changes as per your requirements.
