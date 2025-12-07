# container-isolation-through-dedication-of-networks
Isolating 2 serving applications on the same hosting machine, through facilitating a dedicated customized bridge network (non-default) for each of those serving applications so that they do not communicate with one another

Network-One:
+ Serving application: Devilbox (i.e. a flask-app based on the image: python:3.11-slim)
+ Database: PostgreSQL DB
+ Network: network-one

Network-Two:
+ Serving application: Wordpress CMS (i.e. image: wordpress:latest)
+ Database: MySQL
+ Network: network-two

## Approach
docker-compose (i.e. container running infrastructure-as-code: YAML configuration)

## Acknowledgement of network isolation
```bash
docker network inspect container-isolation-through-dedication-of-networks_network-one
```

```bash
docker network inspect container-isolation-through-dedication-of-networks_network-two
```