# whatsapp-api
whatsapp-api


```python
"""
API: https://rapidapi.com/organization/osint-lite
Help developers and businesses verify whether a phone number is registered on WhatsApp, thereby enhancing the authenticity of the number and effectively reducing potential fraud.
"""
import requests

url = "https://whatsapp132.p.rapidapi.com/open/phone/service-plan"

payload = {
	"phone": "+917428730894",
	"service_plan": 2
}
headers = {
	"x-rapidapi-key": "52eb338445mshe83535e28f8a45ep1934bdjsn7856c9334e81",
	"x-rapidapi-host": "whatsapp132.p.rapidapi.com",
	"Content-Type": "application/json"
}

response = requests.post(url, json=payload, headers=headers)

print(response.json())


```
