Welcome ! You can use my vscode docker image to work on your Java apps !

# onyxia-datascience-images

This docker image is a custom docker images made to use in Onyxia for the [ENSAI](https://ensai.fr/) TD. Simply fill the custom image name to either `odysseu/onyxia-vscode-java:j21` or `odysseu/onyxia-vscode-java:j17` to have respectively java 21 or java 17 pre installed with your VSCode.

<img width="1105" height="726" alt="image" src="https://github.com/user-attachments/assets/88b65d3a-e5ab-417b-872b-590a897af596" />

## Link for docker images

Find the image tags for your docker cli on [Dockerhub : vscode Images with python and java](https://hub.docker.com/r/odysseu/onyxia-vscode-java/tags)

## scheme for what's building

```mermaid
flowchart TB
A[Basic VSC from</br>InseeFrLab]
B[VSC with</br>java 17]
C[VSC with</br>java 21]
A -->|install Java 17</br>& Maven| B
A -->|install Java 21</br>& Maven| C
```
