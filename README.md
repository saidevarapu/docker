docker-compose.yml

services:
   ecomm:
   image: ecomm-app
   build: ecomm-app/
      container_name: ecomm
    ports: 
      - "80:80"

    food:
      image: food-app
      build: food-app/
        container_name: food
      ports:
      - "90:80" 

    login:
       image:
       build:
        container_name: login-con
       ports:
        - "100:80"   