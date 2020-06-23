TICKET GENERATOR
=================

You have been hired as the tech consultant for a local museum in NYC. They are trying to make the experience more efficient for their customers, so they have asked you to create an app that generate tickets for customers based on (1) day of the week, (2) age, and (3) if they have a discount code.

![Beyonce](https://media.giphy.com/media/wJQqAYruWObF7g1W3L/giphy.gif)

GOAL
------------
You want to make an app that takes in the users age, the date of their visit, and whether or not they have a discount. When they hit "Print my Ticket" it should generate their ticket.

![App Demo](https://media.giphy.com/media/J1uCgTBujPzOzyzOiD/giphy.gif)

TASKS
------------
For today's lab you should do the following:  
1. Get the information that the user puts into the form for the date, age, and discount. You should store this information in variables using `document.querySelector`.
2. When the button is clicked, the variables should be updated with the information needed from the form.
**NOTE**: To get the value from a text input field you need to use `.value` with `.document.querySelector()`. For example, to get the value from the day of the week input box you would use:
```javascript
day = document.querySelector("#dayInput").value;
```
3. The museum has the following pricing structure from Wednesday to Monday:

| Age           | Price         |
| ------------- |:-------------:|
| 0 to 5        | Free.         |
| 5 to 18       | $10.          |
| 19 and older  | $20.          |

The museum has the following pricing structure on Tueday's **ONLY**:
| Age           | Price         |
| ------------- |:-------------:|
| 0 to 5        | Free.         |
| 5 to 18       | $5.           |
| 19 and older  | $10.          |

Using conditionals **inside** the event listener for the button, update the values on the ticket at the bottom of the screen with the day, age, and price that the person should pay based on the ticet values above.

EXTENSIONS
------------
The museum is trying to get more people to come visit. If someone uses the code "FREEMONDAYS" and are visiting on a Monday, their ticket is free. If they don't use that code, then they pay the regular price.