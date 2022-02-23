# MoonCatAR

To run locally you need a HTTPS server to allow camera access

## Install http-server globally

`npm i -g http-server`

## Create local cert and key in the root of the repo to use https locally

`openssl req -newkey rsa:2048 -new -nodes -x509 -days 3650 -keyout key.pem -out cert.pem`

## Run the local server with https from the root of the repo where the cert & key is located

`http-server -S -C cert.pem -o`

## View the webpage at 

[https://localhost:8080/ar/demo/index.html](https://localhost:8080/ar/demo/index.html)

## Code is located in 

[https://github.com/vinny-888/MoonCatAR/blob/main/ar/demo/index.html](https://github.com/vinny-888/MoonCatAR/blob/main/ar/demo/index.html)
