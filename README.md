# docker_secrets
## how to protect secrets 
**note don't storing secret in environment variables or source code**
### How to excess environments and secrets 

    docker exec <container _name> env 
    or
    docker run -it --name <container_name> <image_name> sh 
    env
    or
    docker inspect <conatnier_name>
    or
    docker inspect <conatnier_name> {{json .Config.env}}

### Protect your secrets using HashiCorp Vault


