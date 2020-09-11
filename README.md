### GCTExposer - Discover sub-domains by searching through Certificate Transparency logs using Google Transparencyreport


![main](https://raw.githubusercontent.com/m4ll0k/GCTExposer/master/main.png)

![main2](https://raw.githubusercontent.com/m4ll0k/GCTExposer/master/main2.png)

What is CT?
---
Certificate Transparency (CT) is an experimental IETF standard. The goal of it was to allow the public to audit which certificates were created by Certificate Authorities (CA). TLS has a weakness that comes from the large list of CAs that your browser implicitly trusts. If any of those CAs were to maliciously create a new certificate for a domain, your browser would trust it. CT adds benefits to TLS certificate trust: Companies can monitor who is creating certificates for the domains they own. It also allows browsers to verify that the certificate for a given domain is in the public log record.

These logs end up being a gold mine of information for penetration testers and red teams.  

Description by [ct-exposer](https://github.com/chris408/ct-exposer)

Requirements
---

`pip3 install requests` or `python3 -m pip install requests`

Usage
---

```
usage: gctexposer.py [-h] [-i] -d DOMAIN

optional arguments:
  -h, --help            show this help message and exit
  -i, --moreinfo        Show more info..
  -d DOMAIN, --domain DOMAIN
                        Target, e.g: uber.com
```

Example Output
--
![main](https://raw.githubusercontent.com/m4ll0k/GCTExposer/master/main.png)


![main2](https://raw.githubusercontent.com/m4ll0k/GCTExposer/master/main2.png)
