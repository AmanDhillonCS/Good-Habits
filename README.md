# GOOD HABITS 


## Summary
Good Habits is a habit-tracking application that can be used to develop good habits or get rid of bad habits.

Checkout Good Habits app in action - [Good Habits](https://amandhilloncs.github.io/Good-Habits/)
### What is Good Habits?
The main goal of Good Habits is to make an individual complete the tasks they have created. Each task in this context is a habit that a user wants to start or quit. The application will send out notifications at certain time intervals to keep the users on track. The app will also contain a detailed description of ongoing and past activities or habits a user has performed. To keep the person motivated and focused motivational quotes will be sent as notifications throughout the day. Moreover, it will give users a rating on how they are doing towards a habit so they get a sense of achievement and flaunt it among friends.

### Who is it for?
According to Healthline, it takes a person on average about 66 days to develop a regular habit so it is made for people who have trouble developing new habits in a consistent manner, which mostly includes young adults. A person using this application is expected to know how to operate a smart phone. Furthermore, Good Habit is intended for people who lack a feeling of motivation and achievement and want something to push them towards their goals.  

### Why is Good Habits valuable?
Good Habits improves over the traditional mode of tracking a habit which usually involves sticky notes or a notebook. It provides people with reminders so they avoid missing anything and as smart phones are quite handy they can keep track of the progress regularly. Moreover, it provides with motivational quotes to keep individuals focused throughout the day which most other applications lack. It also provides a sense of achievement with its rating system. Overall, during this pandemic, Good Habits can be very valuable for individuals struggling with regular activities.

### What is the success criteria for Good Habits?
Success criteria for Good Habits will be based on three stages. 
* The creation of at least one habit will fulfill the first stage. 
* The second stage can be achieved if the user receives three out of the five rating stars. 
* Finally, the third stage can be reached when the user uses the Good Habits application for more than 66 days as it takes that many days for a habit to become an automatic behavior.

If all these three stages are completed, we can confidently say that the utilisation of this app was successful.

## Architecture
![Architecture](/docs/Architecture3.png)
#### Description 
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

## Velocity 
![Velocity](/docs/Velocity.png)

## Coding Style
### Naming

All shared small variables shall be lowercase 
```
type 
```
All inner class or longer variables names (not shared) shall be camel case.
```
typeGroup
```
All Interface classes and Objects shall start with Capital letter.
```
public interface HabitStorageManager { }
```
```
public class Habit { }
```

 ### Format
 
All opening curly brackets shall sit beside the line, not under, followed by a newline.
```
public boolean getHabitType() { }
```
All indents are four spaces. All indenting is done with tabs.
Matching braces always line up vertically in the same column as their construct.
```
if(condition) {
    do thing
}
```
All classes should look like this:
```
class Habit {
    //fields
    //constructors
    @override
    //methods
    
    //methods
}
```
 

### Documentation

Strict rules for documentation have been used throughout the project. We have avoided self-explainatory comments. For Methods and functions that are logner, complex and require more information we have tried to use as simple vocabulary as we can so that a third person can undertand it with ease.
