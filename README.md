# Angular-Labs

# Setup
$ sudo docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=P@ssw0rd" \
   -p 1433:1433 --name serversql1 --hostname serversql1 \
   -d \
   mcr.microsoft.com/mssql/server:2022-latest
$ sudo docker start -a
$ sudo docker exec -it serversql1 "bash"
$ /opt/mssql-tools/bin/sqlcmd -S localhost -U SA -P "P@ssw0rd"


$ npm install -g @angular/cli
$ npm install
$ ng serve --open 