## Common Docker Commands

### Images

|   |   |
|---|---|
| `docker pull alpine:edge`| Pull image from registry |
| `docker image ls` | List all images |
| `docker build -t <tag-name> .` | Build image |

Build container with arguents
```bash
docker build -t tag1 --build-arg arg1=value1 --build-arg arg2=val2 .
```

### Containers
|   |   |
|---|---|
| `docker ps`| List running containers |
| `docker ps -a` | List all containers |


|   |   |
|---|---|
| `docker run --name <cont name> <image name>`| Run container |
| `docker stop <cont name>` | Stop container |
| `docker start <cont name>` | Start container |
| `docker rm <cont name>` | Remove container |

Docker run options

|   |   |   |
|---|---|---|
| -d | Return back to command line | |
| -p | Port mapping | -p 8080:80 |
| --name | The name of the newly created container | --name brian1 |
| -v | Map volume from local to contianer | -v D:/docker:/user/share/nginx/html:ro |
| -it | Iteract with shell | |
| -e | Set environment variable | -e myenv=myvalue |
| -rm | Remove the container once it stops | |
