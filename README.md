# cacert.pem
Fix cURL error 60 SSL certificate problem


If you are getting the following error message:
```
cURL error 60: SSL certificate problem: unable to get local issuer certificate
```
1. Download **cacert.pem**
2. Put it in: **php\extras\ssl** (if you are using **XAMPP**, put it in: **C:\xampp\php\extras\ssl**)
3. In your **php.ini** set the **curl.cainfo** to the path of the **cacert.pem**. For example:
```
curl.cainfo = "C:\Program Files\PHP\v7.0\extras\ssl\cacert.pem"
```
... or, if you are using **XAMPP**:

```
curl.cainfo = "C:\xampp\php\extras\ssl\cacert.pem"
```
4. Restart your webserver/Apache.
