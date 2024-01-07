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

