# Iteration 1 Worksheet 

#### Adding a feature 
---
Feature Name - [Option to start or quit a habit](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/issues/2)

* We wanted the user to be able to create a habit of their choice and have the flexibility to choose what kind of habit they want to create. 
* User could choose to create a good habit that they want to start or a bad habit they want to quit.
* Radio buttons were used to take the input.



**Link**
<br>[Feature](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/issues/2)
<br>[User Story 1](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/issues/14)
<br>[User Story 2](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/issues/15)
<br>[Merege Request](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/merge_requests/2)

#### Exceptional code 
---
While rendering the list view we wanted to get the names of all the habits created. There might be an instance when our list is empty and getting the name of the object from the list will throw an exception. This is handled by the ```public String[] getAllName() throws Exception``` function in the ```HabitStorage.java```

**Link**
<br>
[Exception code](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/blob/master/app/src/main/java/com/example/goodhabits/Persistence/HabitStorage.java)
<br>[Unit Tests](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/tree/master/app/src/test/java/com/example/goodhabits)

#### Branching 
---
[Branching Strategy](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/blob/iteration-1docs/docs/Branching%20Strategy.md)


#### SOLID Principal Violation
---
Group 1 Violation - Dependency Inversion Principle
The ```ItemList.java``` is dependent on both ```Node.java``` and ```Item.java```.
Creating a ```Node``` and ```Item``` instance in ```ItemList``` is a clear violation of the dependency inversion principle 


**Link**
<br>[Issue](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-1/-/issues/17)
<br>[Commit Link](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-1/-/commit/064facb21c5076a7c693247ba4cb24214810ed08)
### Agile Planning 
---
Initially, our tasks were distributed amongst five people but now that our group consists of four members, we have decided to push the feature [Detailed view of each habit](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/issues/4) to Iteration 2.
<br>No other changes were made to Features or User stories 

**Link**
<br>[Detailed view of each habit](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/issues/4)

