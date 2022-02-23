# MoonCatAR

## Demo

![Demo](https://github.com/vinny-888/MoonCatAR/raw/main/demo_small.gif)

## Live Demo

[https://mooncataverse.com/ar/demo/index.html](https://mooncataverse.com/ar/demo/index.html)

# Setup

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

# References and Inspiration

## MoonCatWalk - used to render the MoonCats Walk Cycles

[https://github.com/vinny-888/mooncat-walkcycle](https://github.com/vinny-888/mooncat-walkcycle)

## AR.js - used for tracking the marker using the camera

[https://github.com/AR-js-org/AR.js](https://github.com/AR-js-org/AR.js)


## VoxelMesh - used to render the MoonCat as a single Mesh (Huge performance boost thanks to this the animations are possible)

[https://r105.threejsfundamentals.org/threejs/lessons/threejs-voxel-geometry.html](https://r105.threejsfundamentals.org/threejs/lessons/threejs-voxel-geometry.html)
