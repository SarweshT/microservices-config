# Microservices Config Repository

This repository contains configuration files for all microservices.

## Setup Instructions

1. Create a new GitHub repository (e.g., `microservices-config`)
2. Push all files from this directory to the repository
3. Update the `config-server/src/main/resources/application.yml` file with your GitHub repository URL:
   ```yaml
   spring:
     cloud:
       config:
         server:
           git:
             uri: https://github.com/YOUR_USERNAME/microservices-config.git
   ```

## Configuration Files

- `user-service.yml` - Configuration for User Service
- `rating-service.yml` - Configuration for Rating Service
- `hotel-service.yml` - Configuration for Hotel Service
- `gateway.yml` - Configuration for API Gateway
