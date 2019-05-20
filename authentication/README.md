## Guides

#### 1. Postgres
       
       steps:
        
           enter database: psql
           
           create db:      "CREATE DATABASE authdb;"
           
           enter:           INSERT INTO roles(name) VALUES('ROLE_USER');
                            INSERT INTO roles(name) VALUES('ROLE_PM');
                            INSERT INTO roles(name) VALUES('ROLE_ADMIN');
                             
           quit database:  "\q"
               
#### 2. Setting up Content-Service

        steps:
            
            edit /resources/application.properties: set up your 'username' and 'password' for postgresql 
            

#### 3. Run

        Intellij - steps: File -> New -> Project From Existing Sources, then click next..
        
        
        Terminal
            steps:
                terminal: "mvn clean install", or "mvn install"
                terminal: "mvn spring-boot:run"
            
#### 4. Testing with Postman
- POST: localhost:8762/api/auth/signup
                                       body/JSON: {
                                                     "name":"greg2",
                                                     "username":"greg2",
                                                     "email":"greg2@gmail.com",
                                                     "role":["user"],
                                                     "password":"password"
                                                   }
- POST: localhost:8762/api/auth/signin
                                       body/JSON: {
                                                  	"username":"greg2",
                                                  	"password":"password"
                                                  }
- POST: localhost:8762/hello/hello2
                                       headers: "Authorization": Bearer 'token received in signin request'

- GET: localhost:8762/content/book/1  
                                       headers: "Authorization": Bearer 'token received in signin request'

- GET: localhost:8762/content/allbooks
                                       headers: "Authorization": Bearer 'token received in signin request'


### References
    
- Project Structure: https://docs.spring.io/spring-boot/docs/current/reference/html/using-boot-structuring-your-code.html