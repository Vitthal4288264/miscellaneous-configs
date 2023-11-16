# Postgre set up
## Steps :
1. ``` docker pull postgres ``` this will the postgres image from docker hub


2. ``` docker run --name postgreDev -e POSTGRES_PASSWORD=P@ssw0rd# -p 5432:5432 -d postgres```  -> once you have the image we can run the image in an container.


3. ```docker exec -it {your-postgres-container} psql -U postgres```
   you need to provide container Id. you will be taken to the psql prompt


4. ```` CREATE DATABASE testdb; ````  run this to create the database.


5. *'\q'* to exit from prompt.


6. To verify the database creation in postgres

   ```docker exec -it c48ac6f1386f psql -U postgres -c "\l"``` 

    **Note:** use **" "** if you are using cmd in windows or else **' '**