
## oracle

host: localhost
port: 1521
database: XEPDB1 (service name)
connection type: Basic
username: SYSTEM
role: Normal
password: <your password>
###
online 
https://localhost:5500/em


docker run -d --name ORCL2 -p 1521 -p 5500 -e ORACLE_PWD=sys123 container-registry.oracle.com/database/express:21.3.0-xe
Note: -d for background check docker comes in health state with docker ps

sunny@Oracle1:~$ docker ps

\CONTAINER ID   IMAGE                                                      COMMAND                  CREATED       STATUS                 PORTS                                                                                      NAMES

888dacf84e76   container-registry.oracle.com/database/express:21.3.0-xe   "/bin/sh -c 'exec $O…"   3 hours ago   Up 3 hours (healthy)   0.0.0.0:32771->1521/tcp, :::32771->1521/tcp, 0.0.0.0:32770->5500/tcp, :::32770->5500/tcp   ORCL2


#rabit:
user:guest
pass:guest