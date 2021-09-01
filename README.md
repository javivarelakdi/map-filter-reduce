# map-filter-reduce

Let's practice using `map`, `filter`, and `reduce`!

* * *

### chaining filter() and map()

Imagine we have a group of users with multiple attributes.

```javascript
var users = [{ firstName: 'Bradley', lastName: 'Bouley', role: 'Full Stack Resident' },
             { firstName: 'Chloe', lastName: 'Alnaji', role: 'Full Stack Resident' },
             { firstName: 'Jonathan', lastName: 'Baughn', role: 'Enterprise Instructor' },
             { firstName: 'Michael', lastName: 'Herman', role: 'Lead Instructor' },
             { firstName: 'Robert', lastName: 'Hajek', role: 'Full Stack Resident' },
             { firstName: 'Wes', lastName: 'Reid', role: 'Instructor'},
             { firstName: 'Zach', lastName: 'Klabunde', role: 'Instructor'}];
```

We're going to send out a message to our users but just need their first name in order to personalize it. 

We want to send out this message just to the Full Stack Residents, telling them what a wonderful job they're doing. 

### .reduce()

To start, let's take this array of words and phrases.

```javascript
var epic = ['a', 'long', 'time', 'ago', 'in a', 'galaxy', 'far far', 'away'];
```

With `.reduce()`, try to combine all of these into a single string! 

Let's get back to our users and see how we can actually set the initial value for our reduce method!

```javascript
var users = [{ firstName: 'Bradley', lastName: 'Bouley', role: 'Full Stack Resident' },
             { firstName: 'Chloe', lastName: 'Alnaji', role: 'Full Stack Resident' },
             { firstName: 'Jonathan', lastName: 'Baughn', role: 'Enterprise Instructor' },
             { firstName: 'Michael', lastName: 'Herman', role: 'Lead Instructor' },
             { firstName: 'Robert', lastName: 'Hajek', role: 'Full Stack Resident' },
             { firstName: 'Wes', lastName: 'Reid', role: 'Instructor'},
             { firstName: 'Zach', lastName: 'Klabunde', role: 'Instructor'}];
```

We want to change up the structure of our users so that we can use the users' full name as the key and have their role as the value. Normally, this would take a lot of looping and initializing some variables. However, with reduce we can set an empty object as our starting point and do it all in a single go! try!