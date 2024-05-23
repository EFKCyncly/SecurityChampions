---
title: Security Requirments
sidebar_label: Security Requirments
---

Defining the security requirments helps you out when performing various security related activities. Defining what is important is essential before trying to map out what can go wrong while trying to secure your systems. Additionally, it will be easier to prioritize security work for you in the future, ex: 
    - Patching vulnerabilities found by (insert system we have here)
    - prioritizing threats as part of the [Threat modeling](google.com)
    - When [Security Testing](google.com) 

## What is security requirments? 
> "[OWASP Proactive Controls](https://owasp.org/www-project-proactive-controls/v3/en/c1-security-requirements)"
> A security requirement is a statement of needed security functionality that ensures one of many different security properties of 
> software is being satisfied. Security requirements are derived from industry standards, applicable laws, and a history of past 
> vulnerabilities. Security requirements define new features or additions to existing features to solve a specific security problem or 
> eliminate a potential vulnerability.

## Security requirments the how? 

It is important to understand that all applications made whithin Cyncly has business objectives and functional requirments. Therefore it is important to understand these so you can ask yourself the question "What can't go wrong", in order to meet these requirments. 

Great way of going about this is to define these requirments in one place. Then gradually work towards having automated test-cases for these requirments.

> ### tip
>
>- Look at [OWASP ASVS](https://raw.githubusercontent.com/OWASP/ASVS/v4.0.3/4.0/OWASP%20Application%20Security%20Verification%20Standard%204.0.3-en.pdf) and find testable security requirements that applies to your application
>- Have a look at our Guidelines

---

> ## TL;DR
>
> **Define security Requirments**
> What are some of the things I care about? 
> Take into account: 
> - Confidentiality 
> - Integrity 
> - Availability
> #### Define compliance Requirments 
> Are there any special requirments that must be met, either Compliance and/or legal?
>
> ---
>
> Input: 
> - Business requirment documents
> - Functional requirments documents 
> - Informaiton security policies
> - Regulatory compliance documents 
> - Security Standards & guidelines 
> - Identity and access management requirments 
>
> Output:
> - Description of the application functionality 
> - List of business objectives 
> - Defintion of the application security and compliance requirments
