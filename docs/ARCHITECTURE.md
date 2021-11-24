# Architecture 

GoodHabits app is based on 3 tier architechture 
* Presentation Layer 
* Logic Layer
* Persistense Layer

### Visualization 
---
#### Iteration 3
![Architecture](/docs/Architecture3.png)
---
#### Iteration 2
![Architecture](/docs/Architecture2.png)
---
#### Iteration 1
![Architecture](/docs/Architecture.png)




### Description 
---
#### **Presentation Layer**
Presentation Layer consists of all the user interaction files 
```
AddActivity 
    Helps to create a new Habit and add it to the list of existing Habits. 
```
```
AllHabitsActivity 
    List view containing all existing Habits.
```
```
MainActivity
    The file for the view for the starting screen of the app.
```
```
ProfileActivity
    Display the profile details of the user.
```
```
ProfileInputActivity
    Helps the user to create profile.
```
```
SettingsActivity
    Helps user to manage the settings related to App.
```
```
DetailActivity
    Displays the detail description about the habit.
```
 


#### **Logic Layer**
Logic layer consists of Time picker files and Object Manager files 
```
DateManager
    Calculates dates passed after a Habit object is created.
```
```
TimeManager
    Helps to display the time in 12-hour format.
```
```
TimePickerFragment
    Widget for picking the time.
```
```
HabitManager
    Links presentation Habit object with persistence storage.
```
```
ProfileManager
    Links presentation Profile object with persistence storage.
```
```
QouteManager
    Manages the daily quotes on the home screen
```
```
HabitAlertReceiver
    Helps in recieving habit notification
```
```
NotificationHelper
    Helps in handling notification alerts
```
```
Notifier
    Sends information about the notification
```
```
RatingManager
    Manages the rating progress bar of the application
```



### **Persistence Layer**
We have database interface and database implementation in Persistence Layer

**Database Interface**
```
HabitStorage
    Storage interface Habit objects.
```
```
ProfileStorage
    Storage interface the Profile object.
```
**Non-persistent Storage**
```
Stub/HabitStorage 
    Handles non-persistent storage of Habit objects.
```
```
Stub/ProfileStorage
    Handles non-persistent storage of Profile objects.
```
**Persistent Storage**
```
HabitSQLite 
    Handles persistent storage of Habit objects.
```
```
ProfileSQLite 
    Handles persistent storage of Profile objects.
```


#### **Objects**
**Domain Objets**
```
Habit
    Habit object.
```
```
Profile
    Profile object.
```
