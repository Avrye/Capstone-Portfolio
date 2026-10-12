# Code Review and Enhancement Plan

## Code Review Presentation Video

[![Watch the Code Review Presentation Walkthrough](https://img.youtube.com/vi/82YfFveFkoU/hqdefault.jpg)](https://www.youtube.com/watch?v=82YfFveFkoU)

---
<details>
<summary><b>Part 1: Software Design and Engineering (CS-320 Contact Managment Application)

## Existing Functionality:

 Acts as a digital address book in Java. It validates incoming user info to prevent crashes. This is done by
   * ensuring IDs are under 10 characters and non-blank
   * The name fits within the size limits
   * Phone numbers are exactly 10 digits
   * Addresses stay under 30 characters

 Service classes store records in memory for:
   * Create
   * Read
   * Update
   * Delete

 or CRUD operaations 

### Code Analysis and Weaknesses: 
 * Architectural bugs and issues with code execution.
 * Inconsistent or missing comments
 * Lack of test coverage ffor invalid inputs
 * IDs are store as Strings, but getter methodsattempted to parse them as integers.
 * Uses an ArrayList with slot index counters, meaning deleting items from the middle shifts index positions and causes errors.
 * Deletes and edits use slow linerar loops insted of direct key lookups

### Planned Enhancements:
 * Keep ID types consistently as Strings
 * Swap the ArrayList out for a HashMap for constant-time lookups without index shifting
 * Expand and tighten unit test coverage.

### Course Outcomes Met: 
* Course Outcome One: Standard-compliant environments and commenting
* Course Outcome Three: Rigorous computer science standards via HashMap transition

</details>
<details>
