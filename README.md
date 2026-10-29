# Experiment 09 — Build a custom application image with Docker

**Student:** [Your name]  
**Register number:** [Your register number]  
**Course:** Collaborative Development and DevOps

## Aim

Package a small Python program into a custom image, run a container from it, and inspect its output.

## Files

- `app.py` — the sample Python application.
- `Dockerfile` — build instructions.
- `.dockerignore` — files excluded from the build context.

## Build and run

From this repository directory:

```sh
docker build -t devops-lab-09:1.0 .
docker image ls devops-lab-09
docker run --name lab09-container devops-lab-09:1.0
docker ps -a
docker logs lab09-container
```

The sample container exits after printing its message. Remove it and the image when finished:

```sh
docker rm lab09-container
docker rmi devops-lab-09:1.0
```

## What to record

Record the image tag, build result, container exit status, and actual program output. Image IDs and build times vary by machine.

## Result

Complete this section after building and running the image locally. No Docker build has been run by this repository setup.

## Reference and attribution

The topic follows the Dockerfile and custom-image theme in [Smirk1308/DevOps_LAB_09](https://github.com/Smirk1308/DevOps_LAB_09). The application, Dockerfile, and guide here are independently written.