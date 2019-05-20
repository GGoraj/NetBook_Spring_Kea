###

## Description
   - Eureka Server is a service that maps requests from Zuul gateway ('Authentication' service)
   to registered micro-services: content, hello, reviews
   
   ### Requirements
   - Java 8

            
   ### Run
   
        Intellij
            steps: 
                File -> New -> Project From Existing Sources, then choose maven, click next..
        
        
        Terminal
            steps:
                terminal: "mvn clean install", or "mvn install"
                terminal: "mvn spring-boot:run"
            