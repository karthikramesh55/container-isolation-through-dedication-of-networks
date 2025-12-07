# container-isolation-through-dedication-of-networks
Isolating 2 serving applications on the same hosting machine, through facilitating a dedicated customized bridge network (non-default) for each of those serving applications so that they do not communicate with one another

Network-One:
+ Serving application: Devilbox/python-flask
+ Database: PostgreSQL DB
+ Network: network-one

Network-Two:
+ Serving application: Wordpress CMS
+ Database: MySQL
+ Network: network-two

## Approach
docker-compose (i.e. container running infrastructure-as-code: YAML configuration)