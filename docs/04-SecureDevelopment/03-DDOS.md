---
title: DOS - Denial of service
sidebar_label: Denial of service
---

All applications exposed on the internet are to a greater or lesser extent vulnerable to "Denial of Service" attacks. The goal of such attacks is to take down the services in question so that no one can use them, not even the intended users. The way this is done is by sending so many requests to the services they are unable to handle and therfore become inaccessible. Such attacks are usually distributed and carried out using a "botnet" that the attacker controls, these attacks are refferred to as "DDOS - Distributed Denial of Service". This makes them more diffcult to protect yourself from, as there could be thousands of devices sending thousands of requests every second.

To limit bruteforcing of logins and resources (which can be looked at as a form of DoS attack) in individual applications, you can implement some form of "rate limiting". For large and distributed DoS attacks, however, only more extensive measures in the runtime environment will suffice. There are a number of measures that can be implemented at different levels of the stack. You can scale up resources, reject traffic based on different patterns or characteristics, and have extensive use of caching. 

THe best way to support the platform in this as an application developer is to create the products in a way that makes them easy to scale. (insert reference: containers and such) it mainly boils down to: 

1. Design your application to withstand restarting.
2. Have good metrics and know your application so that you know when and why it makes sense to sale up. CPU usage is for example not always a good metric to base yourself on, maybe in your case it is better to use the number of connecitons or response time? 
3. Be as stateless as possible 

Add info about how we can create elastic software (containers and such)

