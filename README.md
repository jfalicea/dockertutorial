# Basic Commands 

docker run <image name >
docker run <image name > <command>

## runs all the docker containers on the machine 
docker ps --> used to see what's running or to get an id of a container that is running. 
docker ps -a or --all

# start a container 

docker run = docker create AND docker start

docker start -a <container id>   the "-a" flag provides output from the docker container. ***cannot over ride the default command on a pre-established container. 

# Logs 

docker logs <container id> => gets all the inputs/outputs from a container.

This does not restart or run the container... just shows what happended while it was running. 


# stop a container 

docker stop <container id> (SIGTERM) does clean up and nicely shutsdown
if docker doesnt stop after 10sec it will auto kill. 
docker kill <container id> (SIGKILL) instant stop

Prefer using docker stop command over kill...






