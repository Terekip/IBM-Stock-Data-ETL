 📊 #IBM Stock Data ETL with Alpha Vantage
This project is a simple ETL (Extract, Transform, Load) pipeline built in Python. It pulls stock price data for IBM from the Alpha Vantage API, transforms the raw JSON into structured tabular format using pandas, and loads it into a PostgreSQL database.

💡 What It Does
*Extracts daily, weekly, and monthly time series stock data from Alpha Vantage

*Transforms the data into clean, consistent DataFrames (converting dates, numeric values, and column names)

*Loads the data into a PostgreSQL database, storing each time frequency in its own table:

         *Daily_prices

         *Weekly_prices

         *Monthly_prices


🧰 #Technologies Used
*Python

*Alpha Vantage API – for stock market data

*pandas – for data manipulation

*SQLAlchemy – for database interaction

*PostgreSQL – as the destination database

*dotenv – for secure handling of API and DB credentials


⚙️ #How to Use
1. Set up your environment:

    *Get a free API key from Alpha Vantage

    *Create a PostgreSQL database

    *Store your credentials and API key in a .env file

2. Run the script:

     *The script will automatically pull IBM stock data at three different frequencies and store it in your database.

🔒 #Environment Variables
*All sensitive info (API key and DB credentials) is kept in a .env file to keep it secure and configurable.

📌 #Notes
*Only IBM stock data is fetched by default, but the script can be easily modified to work with other symbols.

*Existing tables are replaced each time the script runs—this is useful for up-to-date snapshots, but not for long-term history tracking.

