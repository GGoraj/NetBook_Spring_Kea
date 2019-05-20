# NetBook Spring Kea Project

## Team:
### Petya   pety0016@stud.kea.dk
### Jeffrey jeff0221@stud.kea.dk
### Eric 
### Gregory grze0203@stud.kea.dk   
## Description
### Spring Microservices Project Created For 'Development of Large Systems' class in Kobenhavns Erhvervsakademi May 2019
### Please see architecture diagram in 'Docs' folder

## Microservices

### content-service | Content delivery service
### authentication  | Service providinng authentication/authorization with Spring Security framework and JWT token.
###                   acting as a Zuul gateway for routing to registered microservices
### eureka-server   | Registrar for NetBook microservices
### hello           | Temporary service providing greeting and service's current port number
###
### reviews-service | Service delivering books reviews, created by Petya
###                 | Github: https://github.com/petya-/netbook-reviews-api.git


## Each microservice folder contains step-by-step guide in 'README.md' file.

##
