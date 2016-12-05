## Housekeep Front End Coding Challenge
A customer wants to schedule a cleaning visit. Create a browser-based application that allows them to see times that are available during a given week, select one, and book in their visit.

Use the mock API that we have set up using Apiary:

http://docs.housekeepavailability.apiary.io/#

There are two endpoints, both of which are documented at the link above. Apiary responds as if it were a real API, but it is not actually performing queries on real data, or writing to a database. It just returns a fixed JSON response to each possible request.

# Requirements:
- The user can specify the duration of the cleaning job that they want to book in hours
- Availability data is requested via GET request to the `/availability/` endpoint defined in Apiary, (see above)
- The data returned describing available start times is displayed in a user-friendly interface. Consider a calendar-type view.
- The user can select an available start timeslot. Timeslots that are not possible are not selectable.
- When the user has selected a timeslot, this is indicated visually.
- The user can then confirm their booking. On confirmation, "POST" to the `/book/` endpoint defined in Apiary, submitting the relevant details of what has been selected.
- Parse the servers response and show what has been booked.

# Notes
- We not looking for anything 'production ready'.
- Spend no more than 3-4 hours on the task, and when you submit the work, describe why you made the choices you did, and what you could do to improve your solution
- Use any frameworks which you're familiar with (we currently use Angular 1.5 at Housekeep)
- Don't worry if you don't get through all the requirements - we mainly want to see the way that you approach problems
- Please use source control (e.g. github) and make regular commits to show your progress
- Things that we look for in good code:
    - Readability
    - Flexibility
    - Testability
    - Extensibility
