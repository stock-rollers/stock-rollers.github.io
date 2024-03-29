# Stock Rollers

## [GitHub](https://github.com/stock-rollers)

### Team Members
* [Andrew Patten- Github](https://github.com/Andpatten), [LinkedIn](https://www.linkedin.com/in/andpatten/)
* [Quentin Dye - Github](https://github.com/Quentin-D-NM), [LinkedIn](https://www.linkedin.com/in/quentindye/)
* [Khasiano Webb - Github](https://github.com/NewbieCoder10), [LinkedIn](https://www.linkedin.com/in/khasiano-webb/) 

## Project Description
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
* Investors - A user that is interested in investing and tracking specific selected stocks by
specifying the price range, and industry. Also, being able to view previous and future outlook
on any specific stock.

* New Investor - A user that is interested in learning about stock information, will be able
to follow other users who have already previously invested. This will allow them to see the
outlook of their investment's, by tracking the previous and future prices to decide what is
best to invest into .

## Stock-rollers
The overview of the Stock-rollers app is that, with this app you will be able to track and keep up
with selected stocks information. Also you will be able to follow users to see what other stocks
would be good to invest in, or just watch for future investments.

[PDF Overview](docs/Stock-rollers(2).pdf) 

  
## Summary of current state of the app
* The current state of the app so far is that, you are able to sign in, using the Google Sign In 
service. Then you are able to navigate from the home page to the search bar view, and the account
tab view. There is a dice roll button located above the profile which when clicked will, roll a
random stock. It will then print a specific stock name on the screen, you can then click on that
and it will pull up the current information for that stock and the hhistory of that stock. The
current state of the graph is that it will update as you slide back and forth from left to right
with updating dates. It will be a stretch goal to possible change the color from settings tab, and
also fix functionality when in landscape view. 

#### Aesthetic/Cosmetic Improvements that would improve the app.
* Change the Main Color of the app, via settings.
* Change the Background-Color of the app, via settings.
* Change the font-type style of the app.
* Create a way to share updates on facebook.

#### Stretch Goals
* We could possible work on the colors if we decide to change them.
* We could possible update the font height when needed/wanted.
* Changing the app to shift when the landscape of the phone is turned.


## Milestone 3
* Team Roster
    * Andrew Patten - Primary role: Project lead and server side developer.  
    * Quentin Dye - Primary role: Server side main developer and android client side developer. 
    * Khasiano Webb - Primary role: UI developer.  
    
* Technical Documentation
    * [Entity Relationship Diagram](docs/erd.md)
    * [DDL](docs/ddl.md)
    * [Outlines of technology stacks-Backend](docs/Backend.md), [Frontend](docs/Frontend.md)
    * [Build Instruction's](docs/BuildInstructions.md)
    * [User Instruction's](docs/UserInstructions.md)
    
* Users Stories, ERD and Wireframes
    * [User stories](docs/user-stories.md)
    * [Wireframes](docs/wireframes.md)
    * [Entity Relationship Diagram](docs/erd.md)
* Entity Classes  
    * [User](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/entity/User.java)   
    * [Stock](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/entity/Stock.java) 
    * [Industry](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/entity/Industry.java) 
    * [History](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/entity/History.java) 
* Repository Interfaces
    * [UserRepository](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/dao/UserRepository.java)
    * [StockRepository](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/dao/StockRepository.java)
    * [IndustryRepository](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/dao/IndustryRepository.java)
    * [HistoryRepository](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/model/dao/HistoryRepository.java)
* REST controllers 
    * [UserController](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/controller/UserController.java)
    * [StockController](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/controller/StockController.java)
    * [IndustryController](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/controller/IndustryController.java)
    * [HistoryController](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/controller/HistoryController.java)
* Application logic services
    * [WorldTradingDataService](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/service/WorldTradingDataService.java)
    * [RequestWorldTradingData](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/service/RequestWorldTradingData.java)
    * [UserService](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/service/UserService.java)
    * [StockrollersServiceApplication](https://github.com/stock-rollers/stockrollers-service/blob/master/src/main/java/edu/cnm/deepdive/stockrollersservice/StockrollersServiceApplication.java)
    
## Tools
* [Draw.io](https://www.draw.io/)
* [Github](https://stock-rollers.github.io/)    


## Resources 
* [Data Model Implementation Scenarios](https://deep-dive-coding-java-cohort-8.github.io/2019/10/17/data-model-implementation-scenarios.html#student-absences-one-to-many-with-dependent-entities)
* [Rubric](https://deep-dive-coding-java-cohort-8.github.io/2019/11/22/capstone-project-milestone-3-rubric)

## Miscellaneous
* [Milestones Checklist](docs/milestones.md)
* [Ground Rules](docs/ground-rules.md)
    
