---
title: Auditlogging
sidebar_label: Auditlogging
---

## What is an audit log
A audit log is primarily the process of documentign activity within software systems used across an organization. Audit logs record the occurrence of an event, the time, user and impacted entity. 

> ### Purpose
> The audit logs should be able to prove, or disprove, whether the user has misused their access. This means we should refrain from using > system\service users when ever possible, or atleast have audit logs which can show who used that account. 

Cyncly needs the opportunity to uncover misuse or suspicious actions that go beyond the needs of the service. the logs will also be used for machine checking of suspicious actions. Cyncly needs these audit logs to pertain to what ever service that is directly affecting business needs and services which is hosted by us. 

Companies that host our software by themselves should also have the opportunity to have audit logs for their own data, so they can uncover misuse or suspicous activity on there own data. 

## What is log-worthy
It is primarily the actions that a user performs in the GUI that are log-worthy. Searching for a person is log-worthy, not the dozens of service calls needed to repond to said action. logs from system and\or service users are therefore not necessary as these cannot be traced back to a specific user.

Does this mean taht services should not log? There are two answers to that question: joint services must log. This is to ensure that if UI applications have no logging, the common service will ensure that the activity is logged. When it comes to all services that are internal to the team, it will be up to the team to find the right place to log in. That could mean that many internal services don't need to log. That said, all internal services that contains sensitive information should log. 

It's important to think about the best place to log. Especially in a microservice architecture, it is important to find the place that has all the necessary context so that the log message contains all the necessary information. There may be cases where it is necessary to log in multiple places to get full context. It may be that one service knows which user the action concerns, but another place knows which action was performed. Basically, the application itself should compile the information into a common log message. If this is not possibel, it must be ensured that the log lines can be correlated afterwards and then the team must contact team audit log so that this can be set up. This is because the logs say nothing about who sens them, and we have a desire to be able to collaborate with the teams, whoever they may be, to make sure that we get all the infor we need, even if it may come from several micro-applications. Since we do not know if it is a microapplication or not, it is difficult for us to know if the log is incomplete or if it is really part of a larger service. 

## What should be logged? 

needs to be determined 

## technical implementation of audit log 

Should be discussed 