# docker-sample
docker-sample

## Building your image
docker build -t node-web-app .

## Run the image
Running your image with -d runs the container in detached mode, leaving the container running in the background. The -p flag redirects a public port to a private port inside the container. Run the image you previously built:
 - docker run -p 49160:8080 -d <your username>/node-web-app

## Print the output of your app:
Get container ID
 - docker ps

Print app output
 - docker logs <container id>
  
## Test
curl -i localhost:49160
