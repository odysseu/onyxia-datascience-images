# onyxia-datascience-images

Custom docker images to use in Onyxia

![You can use this image in onyxia by customising the service image](image.png)

## Link for docker images

Find the image tags for your docker cli on [Dockerhub : vscode Images with python and java](https://hub.docker.com/r/odysseu/onyxia-vscode-java/tags)

## scheme for what's building

```mermaid
flowchart TB
A[Basic VSC from\nInseeFrLab]
B[VSC with\njava 17]
C[VSC with\njava 21]
A -->|install Java 17 &\n install Maven| B
A -->|install Java 21 &\n install Maven| C
```