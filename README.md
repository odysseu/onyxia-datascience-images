# onyxia-datascience-images

Custom docker images to use in Onyxia

## Link for docker images

[Dockerhub > vscode Images with python and java](https://hub.docker.com/r/odysseu/onyxia-vscode-java/tags)

## scheme for what's building

```mermaid
flowchart LR
A[VSC \nde base]
B[VSC avec\njava 17]
C[VSC avec\njava 21]
A -->|install Java 17\n install Maven| B
A -->|install Java 21\n install Maven| C
```