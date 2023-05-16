# Docker CLI

## Commands

**Docker Version überprüfen:**
 ```
 docker --version
 ```

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
