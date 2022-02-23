# Node.Js


### HTTPS

```javascript

const http = require("https");

const options = {
	"method": "GET",
	"hostname": "api.lunarfn.tk",
	"port": null,
	"path": "/",
	"headers": {
		"headers": "idk",
		"useQueryString": true
	}
};

const req = http.request(options, function (res) {
	const chunks = [];

	res.on("data", function (chunk) {
		chunks.push(chunk);
	});

	res.on("end", function () {
		const body = Buffer.concat(chunks);
		console.log(body.toString());
	});
});

req.end();

```


### Request

```javascript

const request = require('request');

const options = {
  method: 'GET',
  url: 'https://api.lunarfn.tk',
  headers: {
    'headers': 'idk her',
    useQueryString: true
  }
};

request(options, function (error, response, body) {
	if (error) throw new Error(error);

	console.log(body);
});

```


### Axios


```javascript

var axios = require("axios").default;

var options = {
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