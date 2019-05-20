# NetBook Spring Kea Project

## Team:
- Petya   pety0016@stud.kea.dk
- Jeffrey jeff0221@stud.kea.dk
- Eric 
- Gregory grze0203@stud.kea.dk   

## Description
### Spring micro-services Project Created For 'Development of Large Systems' class in Kobenhavns Erhvervsakademi May 2019
### Please see architecture diagram in 'Docs' folder

## Content:

- content-service  - Content delivery micro-service
- authentication   - Service providing authentication/authorization with Spring Security framework and JWT token.
                     acting as a Zuul gateway for routing to registered micro-services
- eureka-server    - Registrar for NetBook micro-services
- hello            - Temporary service providing greeting and service's current port number

- reviews-service  - Service delivering books reviews, created with Node.js, LoopBack and MongoDB,
                     developed by Petya Buchkova
                     Github: https://github.com/petya-/netbook-reviews-api.git


## Each micro-service folder contains step-by-step guide in 'README.md' file.

##
