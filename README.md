# multi-01-starting-setup


Build image for backend container. 

For linux systems, you can – starting from major version 20.04 of the docker engine – now also communicate with the host via host.docker.internal. This won't work automatically, but you need to provide the following run flag:

--add-host=host.docker.internal:host-gateway

docker run --name backend-goals --add-host=host.docker.internal:host-gateway --rm goals-node