# Research

Before designing and implementing the agent, I want to first understand the problem we're trying to solve.

## Questions

### The Problem

- Why would we want this?
 - To collect logs across all our machines and services and send it to a centralised location
 - To reduce potential of losing logs in application or network failures
 - To make it easier to find and search through logs when something inevitably breaks
- What problem are we trying to solve?
 - Many machines and many services means many points of failures across many destinations and many time spent trying to debug failures :) 
 - Instead of sshing into these machines and digging through logs, we can store them in a centralised location.
- Whom do you serve? Sauromann
 - Developers who own the services
 - DevOps / Platform engineers who manage the infra those services run on 
 - Cybersecurity engineers who want to monitor logs
 - Alerting and monitoring systems
- What value does it provide?
 - Reliable way for collecting logs across many machines & services 
 - A central location to search through logs and identify patterns
 - Less chance of losing valuable logs when something goes wrong

### Existing Solutions

- How is this problem solved today?
 - Typically, logs are collected by running an agent on the machine producing the logs. The agent collects specific log outputs and then forwards those logs to a central logging platform.
- What existing tools are available?
 - There are a number of tools that solve the same general problem of collecting, processing and forwarding logs to a central location. For this research, i've decided to look at 2 existing tools. Fluentbit and splunk. 
 - The reason for looking at fluentbit is pretty simple, it's the tool that gave me the idea for this project, which I will likely base a lot of my inital designs on. The reason for splunk is less simple. I would typically compare the first existing solution against another solution more directly comparable and look at the different trade offs they make. For this project though, I'd rather look at a tool that shares some similarties, but exists as a much larger ecosystem. Although much of this will likely be out of the scope for this project, this should help shed light on what happens to logs beyond the inital collection.


- What problems do they solve?


### Requirements
