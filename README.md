Docker SCP Server
=================


###Description

SCP server in a docker container allowing anonymous (empty password) authentication.
Docker-Compose gives access to read/save files in the current directory.


###Thanks to:
https://github.com/alphabet5/anonymous-scp-docker


###Run with:
docker-compose up


###Palo Alto SCP Export Example:
scp export configuration remote-port 2222 from running-config.xml to anonymous@w.x.y.z:/scp-server/out.xml


On PAN-OS may need to delete keys with:
delete authentication user-file ssh-known-hosts user ip w.x.y.z username all

