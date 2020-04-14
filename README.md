# nodetest1_csv

Technologies applied: 

Node JS as backend.
ExpressJs as Middleware.
Mongo db in memory server.
Moongose as ORM.
Ejs as view Engine, for SSR.
Routes (MVC pattern)
Controllers (MVC pattern)
Model (MVC pattern)
For testing: JEST (validate we can insert a vehicle data correctly into mongo db).
Style: Custom css, no css framework like boostrsap is must.

The applications has 2 views, first one to upload data and secondly to view which data was uploaded from csv file, to make good front end presentacion, I used cards presentation with own css.

Assumptions:
- According  test requirment app should store all the time 10 columns, then application will only maping those columns, 
if one of then lack then application it´s going to save null over this colum.
App take care only for 10 predefined columns, 
in any columns is not part of then should will be detect and store in an array
(the idea here is in future show up the user which columns was exlcuded from the csv file). To do this validation I used an array located in the path ./utilis/supplierCols.js  as setting file.
