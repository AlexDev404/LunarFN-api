# PowerShell



### Invoke-WebRequest

```powershell

$headers=@{}
$headers.Add("headers", "idk")
$response = Invoke-WebRequest -Uri 'https://api.lunarfn.tk' -Method GET -Headers $headers
```