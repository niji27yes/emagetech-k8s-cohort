# Assignment 01

## Part 1 Reflection:
The Docker commands that were new to me are:
- docker logs. I used this command to get logs of the practice-web container.
- docker container prune. I used to remove stopped containers.
- docker system df. I used to check the disk usage of containers and images.

## Part 2 answers: the three numbered "Question" prompts in Part 2 (images vs containers, run vs exec, the read-only mount flag).
1. After running the four commands above, how many images do you have? How many containers? Why?
- I have two alpine images because the **"docker container run alpine echo hi"** command doesn't specify a tag and so Docker pulled the latest tag and ran the container with it.

2. What's the difference between docker run -it alpine sh and docker exec -it <name> sh? When would you use each?
3. Find the flag that mounts a single file from the host into a container as read-only. (Hint: search for "mount" in the run --help output.)


## Part 3 evidence: a screenshot (or copy-pasted terminal output) showing:
docker container ls after step 3
The browser page after step 8 showing your custom message
The output of docker container inspect -f '{{.NetworkSettings.IPAddress}}' practice-web from step 9
One thing that surprised you about how Docker behaves.
Push the file to your fork of the cohort repo under submissions/assignment-01/ and open a pull request, or post the link in the cohort Slack channel #assignments — whichever your TA prefers.
