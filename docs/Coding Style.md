# Coding Style
## Naming

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

 ## Format
 
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
 

## Documentation

Strict rules for documentation have been used throughout the project. We have avoided self-explainatory comments. For Methods and functions that are logner, complex and require more information we have tried to use as simple vocabulary as we can so that a third person can undertand it with ease.