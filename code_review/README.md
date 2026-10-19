# Code Review and Enhancement Plan

## Code Review Presentation Video

[![Watch the Code Review Presentation Walkthrough](https://img.youtube.com/vi/82YfFveFkoU/hqdefault.jpg)](https://www.youtube.com/watch?v=82YfFveFkoU)

---

<details>
<summary style="display: flex; align-items: center; cursor: pointer;">
  <h2 style="margin: 0; display: inline;">Software Design and Engineering (CS-320 Contact Management Application)</h2>
</summary>

### Existing Functionality:

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

 or CRUD operations 

### Code Analysis and Weaknesses: 

 * Architectural bugs and issues with code execution.
 * Inconsistent or missing comments
 * Lack of test coverage for invalid inputs
 * IDs are stored as Strings, but getter methods attempted to parse them as integers.
 * Uses an ArrayList with slot index counters, meaning deleting items from the middle shifts index positions and causes errors.
 * Deletes and edits use slow linear loops instead of direct key lookups

### Planned Enhancements:

 * Keep ID types consistently as Strings
 * Swap the ArrayList out for a HashMap for constant-time lookups without index shifting
 * Expand and tighten unit test coverage.

### Course Outcomes Met: 

* Course Outcome One: Standard-compliant environments and commenting
* Course Outcome Three: Rigorous computer science standards via HashMap transition

</details>

<details>
<summary style="display: flex; align-items: center; cursor: pointer;">
  <h2 style="margin: 0; display: inline;">Algorithms and Data Structures (CS-300 Course Sorting Application)</h2>
</summary>

### Existing Functionality:
  
  A C++ command-line application that processes a spreadsheet of college courses and builds a custom Binary Search Tree to keep records sorted alphabetically by course ID. Users can interact via a menu to:
  * Load course data from a file
  * Display all courses in alphanumeric order
  * Search for a specific course and view its prerequisites

### Code Analysis and Weaknesses: 
  * Memory Leaks: Tree nodes are allocated on the heap using 'new', but the program never deallocates them when exiting, leaving dangling memory
  * File Reading Bugs: The loader causes some lines to be read twice, creating duplicate or glitchy entries. 
  * Menu Numbers: Menu input checks rely on unmanaged hardcoded number ranges that do not cleanly match menu options. 
  
### Planned Enhancements:
  * Implement a proper recursive destructor to automatically clean up heap memory upon Exit. 
  * Update the file loading loop to check 'getline' directly to prevent duplicate final line reads. 
  * Refine menu input validation and control flow.
    
### Course Outcomes Met: 
  * Course outcome Two: Using well-founded techniques and tools in computing practices.
  * Course outcome Four: Building secure, efficient, and maintainable software solutions (memory management and structured logic).
    
</details>

<details>
<summary style="display: flex; align-items: center; cursor: pointer;">
  <h2 style="margin: 0; display: inline;">Databases / Client-Server Management (CS-340 Python CRUD Module)</h2>
</summary>

### Existing Functionality: 
 
 A Python class that acts as a bridge between client applications and a MongoDB database housing animal shelter records, handling core CRUD operations (Create, Read, Update, Delete) with flexible filtering capabilities. 

### Code Analysis and Weaknesses: 
  * Many Typos and unrefined variables
  * Control flow errors that fail to return data correctly, which defaults to 'None'.
  * Connection strings pass raw credentials without any proper formatting or URL encoding, which can create vulnerabilities if passwords contain special characters.
    
### Planned Enhancements:
  * Fix all typos and ensure that all variables are properly defined
  * Ensure that all data inputs are properly handled to help with security
    
### Course Outcomes Met: 
  * Course Outcome Three: Evaluating solutions using rigorous standards and structured testing. 
  * Course Outcome Five: Protecting data integrity and security through robust database design and defensive programming.
