# Expancer (Expenses for Freelancer)

## What is this

This is an Application written in Java / Typescript to manage expenses.
It is based on microservices (so Springboot + eureka + feign, etc).
Most of the operations are async (for processing) and only the direct client interaction is implemented via REST.  
It has a CICD Pipeline (currently only on my local jenkins). 


Everything is deployed in Docker, for later releases I will prepare template for openshift/OKD and Kubernetes. 
Security is based on keycloak (with OpenID). 

The demo is available on ref.eimantas-services.de (credentials test/test)

Everything is on MIT Licence and hosted on my server.  
So lot of bugs/unimplemented features are expected. As my favourite gaming community says: **Free game, no bitching &trade; /r/dota2**

**However** any PRs / Feature suggestions / Bug reports are greatly appreciated. 

## why I do this? 

Since I became a freelancer, I felt need to manage my financial stuff with some kind of program. I looked in the internet, and I havent found any Free / Opensource solution that provides my needs.  

The requirments are:
* basic management for expenses
* android app and Web Interface
* rest API
* manage multiple accounts
* show what do I have to pay for taxes 
* travelling management (with bookings, hours, etc)
* reporting (in PDF and in Excel)

Additionally, my current position in the Project has not a developer / devops role, so this hobby doesnt allow me forget all the joys of Dev(Ops) (I am Geek by nature)

Currently only some of the points are implemented (I am currently working on it evenings and on weekends) so the pace is not too fast (after all, the journey is the destination), because I have another Project on Full-time. 


## Components

The whole stack (including monitorng/loggin infra) has 14 Servers currently.

* frontend (GIT_URL)
* backend-expenses (GIT_URL)
* backend-accounts (GIT_URL)
* backend-users (GIT URL)
* processing-service (GIT_URL)
* android App (GIT_URL)
* keycloak
* eureka
* jenkins 
* grafana
* prometheus 
* rabbitmq 
* elastic/kibana/logstash
* mysql 


## Target audience - Now

this project is mainly my hobby. So the target audience (currently) are people that can develp / test the software. It can be also used to deploy as an application stack for demo reasons in openshift / kubernetes / docker-compose. It is not ready for the general audience. 

## Target audience - Tomorrow

In future it may be suitable to people who are traveling for work, and want to keep their expenses organized with and have automated tedious work, like reports for business miles. 
Basically everyone who needs some time keeping with expenses tracking along some reporting. 

## Perfomance / HA

TODO

## TODOs

* archicture sketches / overview
* proper GUI (with normal user messages)
* security hardening 
* email functionality 
* extensive configration 
* personalization
* rename components/service to better reflect the purpose of each component
* templates for OKD/Kube/Docker-Compose
