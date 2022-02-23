# Ruby


### net:http

```ruby
require 'uri'
require 'net/http'
require 'openssl'

url = URI("https://api.lunarfn.tk")

http = Net::HTTP.new(url.host, url.port)
http.use_ssl = true
http.verify_mode = OpenSSL::SSL::VERIFY_NONE

request = Net::HTTP::Get.new(url)
request["headers"] = '?'

response = http.request(request)
puts response.read_body
```



### Unirest


```ruby

require 'uri'
require 'net/http'
require 'openssl'

url = URI("https://api.lunarfn.tk")

http = Net::HTTP.new(url.host, url.port)
http.use_ssl = true
http.verify_mode = OpenSSL::SSL::VERIFY_NONE

request = Net::HTTP::Get.new(url)
request["headers"] = '?'

response = http.request(request)
puts response.read_body

```