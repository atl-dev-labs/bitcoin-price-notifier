Bitcoin Price Notifier
"The Tool To Email You When Bitcoin Price Reaches A Certain Amount"

created by:       

ATL DEV LABS
            
Bitcoin is sound money. Meaning that it does not suffer from inflation and cannot be manipulated by a central bank. 
ATL DEV LABS created a python script that sends an email to you whenever the price of bitcoin reaches a value that is input by the user. 

NOTE: This script works via Google Mail only. You have to allow for Less Secure Apps in your Google settings for this script to work. Just set this feature to ‘On’ and everything will work fine. If you have double verification, you cannot do this.

Download the code from the repository and run: 
- python3 bitcoinEmailer.py

The following Python Libraries are used:
- requests
- time
- email.mime
- smtplib

App Outline:

1. You are asked a series of inputs including: your email address (GMAIL only), Gmail password (will be masked), 
   email address to send alert to, and the amount by which you want to be alerted. 
2. Next, it checks the Coinbase API for the current price (updated by the minute on site).
3. If the price of Bitcoin is not below indicated set amount, it will run again in 30 seconds.
4. If it IS below the amount you indicated, it will send you an email alert, and stop running.
