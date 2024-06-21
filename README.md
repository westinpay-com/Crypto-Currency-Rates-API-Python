# Crypto-Currency-Rates-API-Python
WestinPay's Free Crypto API provides real-time cryptocurrency exchange rates and conversions. It's perfect for financial apps, e-commerce platforms, and travel services that integrate cryptocurrency transactions.
# Free Crypto Currency Conversion API

WestinPay’s free API provides access to cryptocurrency exchange rates, ensuring your crypto conversions are quick, accurate, and backed by reliable, up-to-date data.

## WestinPay Crypto Currency Python Code

```python
import requests

api_key = 'your_api_key'
base = 'BTC'
output = 'JSON'
url = f'https://westinpay.com/currency/crypto_api?api_key={api_key}&base={base}&output={output}'

response = requests.get(url)

if response.status_code == 200:
    data = response.json()
    print(data)
else:
    print(f'Error: {response.status_code}')
