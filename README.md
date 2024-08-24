![logo](https://github.com/misbahiradat/Forecasting-of-Currency-Price/blob/main/DALL%C2%B7E%202023-10-31%2017.55.30%20-%20Illustration%20of%20a%20dynamic%203D%20space%20filled%20with%20floating%20bar%20and%20pie%20charts%2C%20all%20showing%20financial%20data.%20Amongst%20these%20charts%2C%20luminous%20currency%20symbol.png)
# Description
The script extracts data from the MetaTrader 5 (MT5) platform and stores it in a database. The data can be extracted for any currency symbol and timeframe.

# Prerequisites
A MetaTrader 5 account is required.
Necessary Python packages, including MetaTrader 5 and SQLAlchemy, must be installed.
# Usage
The script is command-line executable and accepts several arguments:

-s, --symbol: Currency symbol (required).
-t, --timeframe: Timeframe value for data extraction (e.g., M1, D1) (required).
-f, --fromdate: Start date for extraction (optional, defaults to 01-01-2002).
-o, --todate: End date for extraction (optional, defaults to 31-12-2020).

# Examples 
## To extract and store data in a local PostgreSQL database:
python data_extraction.py -s EURUSD -t D1 -f 01-01-2002 -o 31-12-2020
## Accessing the data:
psql -U {USERNAME} -d {database_name}
## To extract and store data as a local CSV file:
python connect_mt5.py -s EURUSD -t D1 -f 01-01-2002 -o 31-12-2020

# Logging
All significant events are logged in the mt5_data_extraction.log file located in the same directory as the script.
# Note
For storing data in PostgreSQL, other scripts (session.py, connect_mt5.py, and engine_pass.py) should be present in the directory.
The script assumes a pre-configured database with connection settings in the session.py file.
Data is stored in tables named using the convention [currency_symbol]_[timeframe_name].




 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
