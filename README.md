# Stock Rollers

## Description
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The Stock Rollers app will help users pick out stocks from desired industries. 
Users will be able to choose what industry they want a stock from and then specify a price range.
After the user is finished selecting parameters, Stock Rollers will display stocks within the specified price range that have also risen 5% within the last 30 days.
The user will then be able to pick from the displayed stocks or let the random number generator pick their stock for them.
The user will be able to either reject or accept the randomly generated stock.
The previously selected stocks will all be displayed as favorites on the users home page along with a link to graph data for each stock.
Stock rollers will not be purchasing the stocks for the user but rather helping the user in choosing the stocks.
All users will have the ability to follow other users that have their profile set to public and see their stock selections. 
Users will be able to view which users are following a particular stock.
In general our app is built to connect new and old investors.
 
 
## Intended Users
* Investors - A user that is interested in investing and tracking specific
selected stocks.
* New Investor - A user that is interested in stock information.

## Milestone 2
* Team Roster
    * Andrew Patten
    * Quentin Dye
    * Khasiano Webb
* Users Stories, ERD and Wireframes
    * [User stories](docs/user-stories.md)
    * [Wireframes](docs/wireframes.md)
    * [Entity Relationship Diagram](docs/erd.md)
* Entity Classes  
    * [User](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/entity/User.java)   
    * [Stock](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/entity/Stock.java) 
    * [Industry](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/entity/Industry.java) 
    * [History](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/entity/History.java) 
    * [DataPoint](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/entity/DataPoint.java) 
* Repository Interfaces
    * [UserRepository](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/dao/UserRepository.java)
    * [StockRepository](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/dao/StockRepository.java)
    * [IndustryRepository](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/dao/IndustryRepository.java)
    * [HistoryRepository](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/dao/HistoryRepository.java)
    * [DataPointRepository](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/dao/DataPointRepository.java)
* REST controllers 
    * [UserController](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/controller/UserController.java)
    * [StockController](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/controller/StockController.java)
    * [IndustryController](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/controller/IndustryController.java)
    * [HistoryController](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/controller/HistoryController.java)
    * [DataPointController](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/controller/DataPointController.java)
* Application logic services
    * [WorldTradingDataService](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/service/WorldTradingDataService.java)
    * [StockRollersDatabase](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/service/StockrollersDatabase.java)
    * [RequestWorldTradingData](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/service/RequestWorldTradingData.java)
    * [StockrollersServiceApplication](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/StockrollersServiceApplication.java)
    
## Tools
* [Draw.io](https://www.draw.io/)
* [Github](https://stock-rollers.github.io/)    


## Resources 
* [Data Model Implementation Scenarios](https://deep-dive-coding-java-cohort-8.github.io/2019/10/17/data-model-implementation-scenarios.html#student-absences-one-to-many-with-dependent-entities)
* [Rubric](https://deep-dive-coding-java-cohort-8.github.io/2019/11/03/capstone-milestone-2-rubric.html)

## Miscellaneos
* [Milestones Checklist](docs/milestones.md)
* [Ground Rules](docs/ground-rules.md)
    
