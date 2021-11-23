# Docker Container Environment
## Project <Docker Compose>

Build Containers For All Mas-Services will be applied
This includes:
* gateway microservice will run in port 7000
* masclient<react-client> will run in port 25566-9000
* maslogin microservice will run in port 9001
* biller microservice will run in port 9002
* applications microservice will run in port 9003
* queries microservice will run in port 9004

# Configurations Database
* MAS_DB_CONNECTION : define connection database
* MAS_MAX_DB_CONNECTIONS : define max dabase connection
* MAS_IDLE_DB_CONNECTION : define idel connection database

```
Note:for testing 
1- Install Docker
2- Run docker compose up
now you can use maxclient application with port in container

## Adding Fields in table<CANCEL_REQUEST>
### TELE, EMAIL, NID, AGREEMENT