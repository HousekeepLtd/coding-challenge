# Housekeep Interview Stage 1: Coding
As a way of assessing your approach to writing software, we'd like to read some of your code.

You have the choice of either:

- Submitting a project that you have previously completed
- Taking the Housekeep coding challenge

The choice is entirely up to you, and what you feel best represents your abilities.

# Submitting existing code
If you have an existing project that you feel represents your abilities, we would love to see it. Here are a few pointers to help you select appropriately:

- Python and/or Javascript/Typescript are preferred, but we'll also consider other languages.
- The ideal submission format is a version-controlled repository, e.g. a Github or Bitbucket repo, but if you cannot share one of these a zipped archive is fine.
- If any part of the code is not your own work, you must indicate this clearly.
- Include a note saying why you are proud of this code, what it does, and why it represents your abilities.
- If a project is very large, point to the parts on which we should focus.


# Housekeep Front End Coding Challenge
Write code to the following specifications.

A customer wants to schedule a cleaning visit. Create a browser-based application that allows them to see times that are available during a given week, select one, and book in their visit.

## API specifications

Create a service that simulates talking to a backend with two endpoints. It's up to you how you do this.

**There is no need to build a backend service - you can simulate making requests and just have your methods return a fixed JSON response.**

### Availability

This "endpoint" should take a duration argument and return a representation of cleaning appointments that are available. Something like:

```js
  mockApiService.getAvailability(duration);
```

You can return the [sample response](availability.json) regardless of the duration supplied.

### Booking

This "endpoint" should receive the time slot that has been selected, and return a response to show the cleaner that has been booked. Something like:

```js
  mockApiService.book({
    "day": "2018-06-08", "start": "19:00:00", "end": "22:00:00"
  });
```

You can return the [sample response](booking.json) regardless of the arguments supplied.

## Requirements:
- The user can specify the duration of the cleaning job that they want to book in hours
- Availability data is requested via your mock service (see above)
- The data returned describing available start times is displayed in a user-friendly interface. Consider a calendar-type view.
- The user can select an available start timeslot. Timeslots that are not possible are not selectable.
- When the user has selected a timeslot, this is indicated visually.
- The user can then confirm their booking. On confirmation, simulate posting to the server using your mock service, submitting the relevant details of what has been selected.
- Parse the response and show what has been booked.

## Notes
- We not looking for anything 'production ready'.
- Spend no more than 3-4 hours on the task, and when you submit the work, describe why you made the choices you did, and what you could do to improve your solution
- Use any frameworks which you're familiar with (we currently use Angular 6 at Housekeep)
- Don't worry if you don't get through all the requirements - we mainly want to see the way that you approach problems
- Please use source control (ideally github) and make regular commits to show your progress
- Things that we look for in good code:
    - Readability
    - Flexibility
    - Testability
    - Extensibility
