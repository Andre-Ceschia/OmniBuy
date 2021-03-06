# OmniBuy
OmniBuy is a trading bot that is able to utilize multiple trading strategies to optimize profits. It is able to trade many readily available cryptocurrencies. OmniBuy utilizes both the TradingView API, for technical analysis, and KuCoin API, for placing orders. 
 
Prerequisites:
  - A Google Account
  - A KuCoin Account

Google Sheet Setup:
  - Go to https://console.cloud.google.com/
  - Create a project
  - Click "Go to APIs overview"
  - Click "Library"
  - Search for "Google Drive"
  - Enable "Google Drive"
  - Navigate to "Credentials" inside of the "Google Drive API" settings
  - Click "Manage Service Accounts"
  - Click "Create Service Account"
  - Name the service account
  - Give the service account the role of "Editor"
  - Click "Done"
  - Click the three dots underneath the "Actions" column of the service account
  - Click "Manage Keys"
  - Click "Create New Key", and select "JSON"
  - Rename the file to "creds.json"
  - Navigate to the library in API overview
  - Search for "Google Sheets API"
  - Enable the "Google Sheets API"
  - Open the "creds.json" file and copy "cilent_email" to your clipboard
  - Go to your Google Drive and create a new Google Sheet
  - Create the headers, "Date", "Time Bought", "Time Sold", "Fees Paid", "Profit", "Profit(%)", "Buy Price", "Sell Price", and "Trading Pair"
  - Share the Google Sheet with the email you copied in the previous step
  
KuCoin API Setup:
  - Go to https://www.kucoin.com, and log in
  - Navigate to "API Management"
  - Create an API Key with the "Trade" option enabled
  - Save the API key, secret, and passphrase 
 
OmniBuy Setup:
  - Git Clone this repository to the folder of your choice
  - Move "creds.json" to the "src" subfolder
  - Navigate to the OmniBuy folder in a terminal
  - In the terminal enter the command "pip install -r requirements.txt"
  - Navigate to the "src" folder
  - Enter "python Main.py" to start OmniBuy
  - Enter your KuCoin API, key, secret, and passphrase when prompted
  - Enter the name of the Google Sheet created in the previous steps when prompted
  - Enter "Help" in the OmniBuy terminal for any further assistance

# Warning
USE AT YOUR OWN RISK, I AM NOT A FINANCIAL ADVISOR, I AM NOT AT FAULT FOR ANY LOSS OF CAPTIAL YOU ENDURE FROM UTILIZING OMNIBUY
