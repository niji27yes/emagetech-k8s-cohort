# Assignment 01

## Part 1

The Docker commands that were new to me are:
- docker logs. I used this command to get logs of the practice-web container.
- docker container prune. I used to remove stopped containers.
- docker system df. I used to check the disk usage of containers and images.

## Part 2

1. After running the four commands above, how many images do you have? How many containers? Why?
- I have two alpine images and one container because the **"docker container run alpine echo hi"** command doesn't specify a tag and so Docker pulled the latest tag and ran the container with it.

2. What's the difference between **docker run -it alpine sh** and **docker exec -it <name> sh**? When would you use each?
- **docker run -it alpine sh** opens an interactive session in a running container and is used when you need to access a running container and execute commands in it.
- **docker exec -it <name> sh** excutes a command inside a running container and is used when you need to execute a command or script inside a running container without creating an interactive session.

3. Find the flag that mounts a single file from the host into a container as read-only. (Hint: search for "mount" in the run --help output.)
- **--mount** with **readonly** or **-v** with **:ro**

## Part 3

1. docker container ls after step 3
  > <img width="1502" height="187" alt="image" src="https://github.com/user-attachments/assets/58dbe2fc-8817-43f5-9c8a-29d53c576162" />  


2. The browser page after step 8 showing your custom message
  <img width="1406" height="459" alt="image" src="https://github.com/user-attachments/assets/bf898d79-add2-45de-a420-c16e21ec7101" />


3. The output of docker container inspect -f '{{.NetworkSettings.IPAddress}}' practice-web from step 9
  <img width="1113" height="90" alt="image" src="https://github.com/user-attachments/assets/e5ce1270-0b1a-4c55-9ba9-b515819462ff" />


4. One thing that surprised you about how Docker behaves.
- How some commands are aliased out the box.
