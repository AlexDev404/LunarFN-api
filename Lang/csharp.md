# C Sharp

### Restsharp:

```csharp
var client = new RestClient("https://api.lunarfn.tk");
var request = new RestRequest(Method.GET);
request.AddHeader("uhhh Headers?");
IRestResponse response = client.Execute(request);
```


### HttpClient:

```csharp
var client = new HttpClient();
var request = new HttpRequestMessage
{
    Method = HttpMethod.Get,
    RequestUri = new Uri("https://api.lunarfn.tk"),
    Headers =
    {
        { "uhhh Headers?" },
    },
};
using (var response = await client.SendAsync(request))
{
    response.EnsureSuccessStatusCode();
    var body = await response.Content.ReadAsStringAsync();
    Console.WriteLine(body);
}
```


### Unirest:

```csharp
var client = new RestClient("https://api.lunarfn.tk");
var request = new RestRequest(Method.GET);
request.AddHeader("headers?");
IRestResponse response = client.Execute(request);
```