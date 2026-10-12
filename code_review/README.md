# Code Review and Enhancement Plan

## Code Review Presentation Video

[![Watch the Code Review Presentation Walkthrough](https://img.youtube.com/vi/82YfFveFkoU/hqdefault.jpg)](https://www.youtube.com/watch?v=82YfFveFkoU)

## Part 1: Software Design and Engineering (CS-320 Contact Managment Application)

### Existing Functionality:

Acts as a digital address book in Java. It validates incoming user info to prevent crashes. This is done by
* -ensuring IDs are under 10 characters and non-blank
* -The name fits within the size limits
* -Phone numbers are exactly 10 digits
* -Addresses stay under 30 characters

Service classes store records in memory for:
* -Create
* -Read
* -Update
* -Delete
or CRUD operaations 

