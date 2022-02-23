# Pyhton


### Requests

```pyhton

import requests

url = "https://api.lunarfn.tk"

headers = {
    'headers': "idk",
    }

response = requests.request("GET", url, headers=headers, params=querystring)

print(response.text)
```