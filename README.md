# docker-all-cheat-sheet

# docker compose build
- sudo docker-compose build
# docker compose start
- sudo docker-compose up
- sudo docker-compose up -d (detached mode)
# docker compose stop
- sudo docker-compose down

# docker image list show
- sudo docker image ls
# docker remove image  
- sudo docker rmi image_id/image_name
# docker force remove image 
- sudo docker rmi -f image_id/image_name
# docker remove all images 
- sudo docker rmi $(sudo docker images -q)
# docker remove dangling images
- sudo docker images -f dangling=true
# docker remove all images(with running images)
- sudo docker image prune -a

# docker running container list show
- sudo docker ps
# docker all container list show
- sudo docker ps -a
# docker container inspect
- sudo docker exec -it container_id/container_name sh
# docker remove container  
- sudo docker rm container_id/container_name
# docker force remove Container  
- sudo docker rm -f container_id/container_name
# docker remove all container
- sudo docker rm $(sudo docker ps -aq)
# docker remove all stopped containers
- sudo docker rm $(sudo docker ps -aq --filter  status="exited")
# docker remove all container(with running container)
- sudo docker container prune

# docker create network
- sudo docker network create network_name
# docker all network list show
- sudo docker network ls
# docker network inspect
- sudo docker network inspect network_id

# docker volume list show
- sudo docker volume ls
# docker volume create
- sudo docker volume create volume_name
# docker remove volume 
- sudo docker volume rm volume_name
# docker remove all volume
- sudo docker volume prune

 