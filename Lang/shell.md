# Shell

### cURL

```shell
curl --request GET \
	--url 'https://api.lunarfn.tk' \
	--header 'headers?'
```


### Wget

```shell
wget --quiet \
	--method GET \
	--header 'headers?' \
	--output-document \
	- 'https://api.lunarfn.tk'
```


### HTTPie

```shell
http GET 'https://api.lunarfn.tk'
```