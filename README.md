# nodetest1_csv

Technologies applied: 

Mongo db in memory server.
Moonse as ORM.
Ejs as view Engine, for SSR.
Routes (MVC pattern)
Controllers (MVC pattern)
Model (MVC pattern)
For testing: JEST (validate we can insert a vehicle data correctly into mongo db).

The applications has 2 views, firt one to upload data and secondly to view which datas uploads from csv using cards presentation.

Assumptions:
- According  test requirment app should store all the time 10 columns, then application will only maping those columns, 
if one of then lack then application it´s going to save null over this colum.
App take care only for 10 predefined columns, 
in any columns is no part of then should be detect and store in an array
(the idea here is in future show up the user which columns was exlcuded from the csv file). To do this validation I used an array located in the path ./utilis/supplierCols.js  as setting file.
