# Iteration 2 
---
### Paying off technical debt 
* We used instances of storage class in iteration 1 but we later changed them into interfaces which are implemented by multiple classes.  
[HabitStorageI and ProfileStorageI](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/tree/master/app/src/main/java/comp3350/goodhabits/Persistence)  

* We didn't have enough tests coverage in iteration 1 but we increased that in iteration 2. This helped us to code more defensively.



### SOLID
Violation of Dependency Inversion Principle as ```HomeFragment.java``` is dependent on ```PetFakeDatabse.java```. Recommended use of Dependency Injection whichi is define the ```PetFakeDatabase.java```
* [SOLID Violation Issue](https://code.cs.umanitoba.ca/3350-winter-2021-a03/minipets-comp3350-a03-group12/-/issues/32)
* [Commit](https://code.cs.umanitoba.ca/3350-winter-2021-a03/minipets-comp3350-a03-group12/-/commit/d0c00824a2c49889075ed91133d70aa2c58ffd61)
### Retrospective 
* [Retrospective](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/blob/master/docs/Retrospective.md)  

### Design Pattern
**Singleton**  
We are using Singleton design pattern in ```HabitSQLite``` and ```ProfileSQLite```. As we create a single instance of ```HabitSQLite``` and ```ProfileSQLite``` using ```onCreate``` method for global access where it behaves as our database driver class and stores data about ```Habit``` and ```Profile``` objects. Positive side of this design pattren is that we can get data anytime we want from this Singleton class.  

[HabitSQLite](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/blob/master/app/src/main/java/comp3350/goodhabits/Persistence/SQLite/HabitSQLite.java)    
[ProfileSQLite](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/blob/master/app/src/main/java/comp3350/goodhabits/Persistence/SQLite/ProfileSQLite.java)  


### Iteration 1 Feedback fixes 
* Removed ```com.example``` portion  
 [Refactor Link](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/tree/master/app/src/main)  


* We pushed rest of the fixes in Iteration 3 as explained in Retrospective.