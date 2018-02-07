# Housekeep Interview Stage 1: Coding
As a way of assessing your approach to writing software, we'd like to read some of your code.

You have the choice of either:

- Submitting a project that you have previously completed
- Taking the Housekeep coding challenge

Both options are described below.


# Submitting existing code
If you have an existing project that you feel represents your abilities, we would love to see it. Here are a few pointers to help you select appropriately:
- Python and/or Javascript are preferred, but we'll also consider other languages.
- The ideal submission format is a version-controlled repository, e.g. a Github or Bitbucket repo.
- If any part of the code is not your own work, you must indicate this clearly.
- Include a note saying why you are proud of this code, what it does, and why it represents your abilities.
- If a project is very large, point to the parts on which we should focus.


# Housekeep Front End Coding Challenge
Write code to the following specifications.

A customer wants to schedule a cleaning visit. Create a browser-based application that allows them to see times that are available during a given week, select one, and book in their visit.

Use the mock API that we have set up using Apiary:

http://docs.housekeepavailability.apiary.io/#

There are two endpoints, both of which are documented at the link above. Apiary responds as if it were a real API, but it is not actually performing queries on real data, or writing to a database. It just returns a fixed JSON response to each possible request.

## Requirements:
- The user can specify the duration of the cleaning job that they want to book in hours
- Availability data is requested via GET request to the `/availability/` endpoint defined in Apiary, (see above)
- The data returned describing available start times is displayed in a user-friendly interface. Consider a calendar-type view.
- The user can select an available start timeslot. Timeslots that are not possible are not selectable.
- When the user has selected a timeslot, this is indicated visually.
- The user can then confirm their booking. On confirmation, POST to the `/book/` endpoint defined in Apiary, submitting the relevant details of what has been selected.
- Parse the server's response and show what has been booked.

## Notes
- We not looking for anything 'production ready'.
- Spend no more than 3-4 hours on the task, and when you submit the work, describe why you made the choices you did, and what you could do to improve your solution
- Use any frameworks which you're familiar with (we currently use AngularJS, Angular 5, and Ionic at Housekeep)
- Don't worry if you don't get through all the requirements - we mainly want to see the way that you approach problems
- Please use source control (ideally github) and make regular commits to show your progress
- Things that we look for in good code:
    - Readability
    - Flexibility
    - Testability
    - Extensibility
