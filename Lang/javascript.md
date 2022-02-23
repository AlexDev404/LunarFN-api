# Javascript


### jQuery

```javascript
const settings = {
	"async": true,
	"crossDomain": true,
	"url": "https://api.lunarfn.tk",
	"method": "GET",
	"headers": {
		'headers': 'idk her',
	}
};

$.ajax(settings).done(function (response) {
	console.log(response);
});
```




### Axios

```javascript
import axios from "axios";

const options = {
  method: 'GET',
  url: 'https://api.lunarfn.tk',
  headers: {
    'headers': 'idk her',
  }
};

axios.request(options).then(function (response) {
	console.log(response.data);
}).catch(function (error) {
	console.error(error);
});
```