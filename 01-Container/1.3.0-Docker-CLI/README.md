# Docker CLI

## Commands

**Docker Version überprüfen:**
 ```
 docker --version
 ```
***

**Docker Image auf Docker-HUB suchen:**

```
docker search <name oder suchobjekt>
```
***

**Docker Image herunterladen:**

```
docker pull <ausgewähltes image>
```
Beispiel: 
```
docker pull <ubuntu/nginx>
```
***

**Container starten mit dem heruntergeladenen Image:**
```
docker run --name <name> -p <port> -d <image>
```
Beispiel:
```
docker run --name container1 -p 80:8080 -d ubuntu/nginx
```

*** 


**Status vom Container überprüfen:**

```
docker inspect -f '{{.State.Status}}' <container name>
```
Beispiel:
```
docker inspect -f '{{.State.Status}}' container1
```

***

**Öffnen Sie eine interaktive Shell im Docker-Container**

```
docker exec -it <container name> /bin/bash
```
Beispiel:
```
docker exec -it container1 /bin/bash
```

***

**Beenden Sie die interaktive Shell im Docker-Container:**
Tastenkombination: Ctrl + d


***

**Stoppen Sie den Container:**

```
docker stop <container name>
```
Beispiel:

```
docker stop container1
```

***

**Überprüfen Sie die Liste der gestoppten Container:**

```
docker ps
```

***

**Entfernen Sie den gestoppten Container:**

```
docker rm <container name>
```
Beispiel:
```
docker rm container1
```