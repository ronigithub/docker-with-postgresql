| Description | Instruction |
|-------------|-------------|
| Pull postgres image | docker pull postgres:<version> |
| start a postgres instance | docker run --name <any_name> -e POSTGRES_PASSWORD=<password> -d -p 5432:5432 postgres:<version> |
| Example | sudo docker run --name vatonlinedb  -e POSTGRES_PASSWORD=<password> -d -p 5432:5432 postgres:10.10-alpine |
| Now login into docker postgres with this command | sudo docker exec -it vatonlinedb bash |
| logged in user postgres | psql -U postgres |
| Check it superuser | \du |
| Now created DB and so on with sql command |
