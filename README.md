# Assessement
This is a Spring Boot application for fetching, caching, and converting currency exchange rates. It uses Redis for caching and provides a REST API for accessing the exchange rates and converting currencies.


## Architecture 
![image](https://github.com/lgsurith/spring-currency-convertor/assets/117572209/13e4d41b-8f7e-4239-8a20-becc4330371b)

## Installation

- Link
  ```bash
  https://github.com/DineshMahendran-2001/assessment
  ```
## Configuration
- Make sure to setup the dependencies as given in the list from [Spring initializer](https://start.spring.io/) or directly from the IDE.
  
  ```
  * Spring Web
  * Spring Data Redis
  * Spring Boot Devtools
  * Spring WebFlux (Spring Reactive Web)
  ```
- The given application must also be configured by ```application.properties``` in src/main/resources/application.properties
  
  ```bash
  spring.application.name=exchangerates

  #to setup external api configs.
  exchange.api.key = your_api_key
  exchange.api.url = https://v6.exchangerate-api.com/v6/
  exchange.api.defaultcurrency = USD
  
  #spring redis setup
  spring.redis.host = your_redis_host
  spring.redis.port=your_redis_port
  spring.redis.username= your_redis_username
  spring.redis.password= your_redis_password
  spring.redis.ssl = true
  ```

## Endpoints

| Endpoint           | Description                                                                                  |
|--------------------|----------------------------------------------------------------------------------------------|
| `/api/exchange/rates` | Obtains Realtime Rates of listed currencies.                                       |
| `/api/exchange/convert`  | Converts any amount of currency to another using querying technique  |


## Results

- Getting Real time rates :

  ![image](https://github.com/lgsurith/spring-currency-convertor/assets/117572209/e9701bde-1d07-44e5-ba85-7ffd53df096e)


- Conversion of Currency Rates :

  ![image](https://github.com/lgsurith/spring-currency-convertor/assets/117572209/56d1bf85-176a-44d4-b2c4-f5c4fef5170f)

- Redis Cache DB :

  ![image](https://github.com/lgsurith/spring-currency-convertor/assets/117572209/a1e9407b-fef5-4919-8fbb-f20d9ec753f2)

  

  



