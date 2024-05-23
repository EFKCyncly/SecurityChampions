---
title: Dynamic analytics
sidebar_label: Dynamic analytics
---

Dynamic analysis (DAST) means analyzing a fully running instance of an app. This is a "black box" test, i.e You don't necessarily know anything about how the app is structured. You communicate with the app via its interface in the same way that an end user\attacker would. THe test tools send (invalid) input that the app wouldn't have gotten during normal use to see how it responds. In this way, both known and unknown weaknesses can be detected. If the app requires login, you can choose whether you want to run a scan with or without valid credentials. 

THe advantage of DAST is that it can detect many types of vulnerabilities that static analysis cannot: various types of injection, denial of service, corss-site scripting, remote code execution, server-side request forgery, insecure direct object references, and many more. Since they attack "from the outside", they can be used regardlesss of the languages and frameworks the app is made of. 

THe disadvantage of DAST is that it is more complicated to set up: Your need to have a production-like environment where the app and its dependencies are set up. The capabilities vary between different tools. For example, not everyone is as smart when it comes to understanding web applicaitons with a lot of JavaScript and complicated flows with XSRF and CSRF tokens. 

DAST tools come in all possibel varieties and price ranges. Some are more or less fully automatic, while others are run manually. Some are installed "on-prem", while others are "As a service" in the cloud. Of the more well-known ones, [Netsparker](https://www.netsparker.com/), [Nessus](https://www.tenable.com/products/nessus) and [Detectify](https://detectify.com/) and many other. 

You can also find vulnerabilities by testing manually. Browsers with developer tools allow you to edit and send requests, as do tools like [curl](https://curl.se/). It can also be useful to use dedicated attack proxy such as [Burp Suite](/SecurityChampions/docs/resources/learningMaterial#portswigger-security-academy) or [OWASP ZAP](https://www.zaproxy.org/). If you want to "fuzz" the app (i.e. send random data to it), tools like [Wfuzz](https://github.com/xmendez/wfuzz) and [FFUF](https://github.com/ffuf/ffuf) can be useful.

You can find a lot of snacks just by rummaging around in your own apps. "What happens if I submit a negatice number for year of birth? What if I submit a string of 4 000 characters instead of the expected 8?. Be curious!
