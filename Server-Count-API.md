# Getting your Authorization Token

To start using server counts on a bot, go to your bot edit page, and click the `Authorization Token` link at the bottom of the page. This will generate an auth token.

# Posting Stats

NodeJS
```js

var requestOptions = {
  method: 'POST',
  headers: {
    "authorization": "YOUR_AUTH_TOKEN",
    "Content-Type": "application/json"
  },
  body: JSON.stringify({"server_count": 1500}); // Replace this number with the server count
};

fetch("/api/auth/stats/:botid", requestOptions) // Make sure you include the domain
  .then(response => response.text())
  .then(console.log)
  .catch(console.error);
```
Python
```py
url = "/api/auth/stats/:botid" # Make sure you include the domain

payload = "{\"server_count\": 1500}" # Replace this number with the server count
headers = {
  'authorization': 'YOUR_AUTH_TOKEN',
  'Content-Type': 'application/json'
}

response = requests.request("POST", url, headers=headers, data = payload)
print(response.text.encode('utf8'))
```

cURL
```bash
curl -H "Content-Type: application/json" \
     -H "Authorization: YOUR_AUTH_TOKEN" \
     -X POST \
     -d '{\"server_count\": 1500}' \
      "/api/auth/stats/:botid"

# Make sure you include the domain and replace the number with the server count
```