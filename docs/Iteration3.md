# Iteration 3 Worksheet

### Note for Marker 
* Integration tests are done in ```androidTest``` folder.
* [Test Folder](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/tree/master/app/src/androidTest/java/com/example/goodhabit)
### What technical debt has been cleaned up?
Our ```HabitManager``` and ```ProfileManager``` were being initialized using constructors, which is not a characteristic of a ```Singleton Design Pattern```. This has been fixed by using a public method to initialize the private variables.

[commit](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/commit/6da6ad8895d215d65fe742393c398f4e352fa28f)

### What technical debt did you leave?
**Deliberate Prudent**

Every ```object``` of ```Notifier Class``` is initialized with a ```Context```, which we cannot get in a ```non-activity class ```. This limits us from using instances from this class in a more flexible way. 

### Discuss a Feature or User Story that cut/re-prioritized
As three features from iteration 2 were pushed to iteration 3 two features from iteration 3 [Dark mode](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/issues/12) and  [Daily task schedule](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/issues/11) were dropped. Both these features had low to medium priority which didn't impact the overall core of the project.

### Acceptance test/end-to-end
**End-to-end Acceptance test for adding a habit**
* First we bypass the login with fake email and name, which we do in the ```setUp``` function of test class.
* Once we reach the ```Home screen``` we make sure that we have exactly three habits in our list. Then we tap the Add button which takes us to the Add Habit screen. 
* Next step is to fill out the Add Habit form by using hard coded data to create a Habit.
* Finally we tap the Submit button and this adds the habit to the list and takes us back to the ```Home screen```.
* Now we check the number of habits again and make sure we have exactly four habits.
* Since, we verify that the number of habits in the list increases by one and the data to create the habit was hard coded by us, the test should always pass and not be flaky.
* Note: We used espresso library for this testing.
* [Test Link](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/blob/c64cb7583998e04479582b1c138fa634aa3b3845/app/src/androidTest/java/com/example/goodhabit/SystemTests/AddHabitST.java)

### Acceptance test, untestable
We could not test the UI notifications for the application because notifications popup with respect to a particular time and this can be very time consuming.

### Velocity/teamwork
![Velocity](docs/Velocity.png)
Over-all throughout the project our esitmates were fairly accurate and got better execpt for iteration 2. As in iteration 2 we had trouble implementing database and with same reason some tasks were pushed to iteration 3. Velocity chart accuratly describes our work that was commmited and work that was done.

### Retrospective

[Retrospective](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/blob/master/docs/Retrospective.md)

### Architecture

[Architecture](https://code.cs.umanitoba.ca/3350-winter-2021-a02/group-12/good-habits-a02-12/-/blob/master/docs/ARCHITECTURE.md)
