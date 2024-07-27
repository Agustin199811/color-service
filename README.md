# Color Service for E-commerce Application

This project is a Color Service for an e-commerce clothing application. The Color Service is designed to manage product colors, allowing other microservices within the platform to effectively interact with color data. By centralizing color management, it ensures consistency and accuracy in the representation of colors across the e-commerce platform.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Running the Service](#running-the-service)
- [Contributing](#contributing)
- [License](#license)

## Overview

The Color Service is a RESTful API built using Spring Boot. It provides endpoints for creating, updating, retrieving, and deleting product colors. This service plays a crucial role in the product management system by ensuring that color data is uniformly managed and easily accessible to other microservices.

## Features

- **Create Colors:** Allows the creation of new product colors with detailed descriptions.
- **Retrieve Colors:** Enables fetching details of existing colors, supporting features like product filtering and search.

## Prerequisites

- Java 17 or higher
- Maven 3.6.3 or higher
- Spring Boot 3 or higher

## Installation

1. Clone the repository:

    - ```sh
      git clone https://github.com/Agustin199811/color-service.git
      cd color-service
      ```

2. Build the project using Maven:

    - ```sh
      mvn clean install
      ```

## Configuration

The configuration for the Color Service is located in `src/main/resources/application.properties`. Below is an example configuration:

```properties
spring.datasource.url=jdbc:mariadb://clot-mariadb.cp88o8squjfi.us-east-1.rds.amazonaws.com:3306/clot
spring.datasource.username=root
spring.datasource.password=root1234

eureka.client.service-url.defaultZone=http://clot-ecommerce-ELB-1792240696.us-east-1.elb.amazonaws.com:8761/eureka/
eureka.client.register-with-eureka=true
eureka.client.fetch-registry=true
```

## Running the Service

To run the service registry, use the following command:

 ```sh
    mvn spring-boot:run
```

## Contributing

Contributions are welcome! If you would like to contribute to this project, please send us an email at
`toapantaagustin9c@gmail.com` with details about your proposed changes or improvements. We look forward to hearing from you!

## License

This project is licensed under the MIT License - see the LICENSE file for details.
