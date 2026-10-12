# Code Review and Enhancement Plan

## Code Review Presentation Video

[![Watch the Code Review Presentation Walkthrough](https://img.youtube.com/vi/82YfFveFkoU/hqdefault.jpg)](https://www.youtube.com/watch?v=82YfFveFkoU)

---

<details>
<summary style="display: flex; align-items: center; cursor: pointer;">
  <h2 style="margin: 0; display: inline;">Part 1: Software Design and Engineering (CS-320 Contact Management Application)</h2>
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
<summary style="display: flex; align-items: center; cursor: pointer;">
  <h2 style="margin: 0; display: inline;">Part 2: Algorithms and Data Structures (CS-300 Course Sorting Application)</h2>
</summary>

### Existing Functionality:
  
  A C++ command-line appliction that processes a spreadsheet of college courses and builds a custom Binary Search Tree to keep records sorted alaphabetically by course ID. Users can interact via menu to:
  * Load course data from a file
  * Display all courses in alphanumeric order
  * Search for a specific course and view its prerequisites

### Code Analysis and Weaknesses: 
  * Memory Leaks: Tree nodes are allocated on the heap using 'new', but the program never deallocates them when exiting, leaving dangling memory
  * File Reading Bugs: The loader causes some lines to be read twice, creating duplicate or glitichy entries. 
  * Menu Numbers: Menu input checks rely on unmanaged hardcoded number ranges that do not cleanly match menu options. 
  
### Planned Enhancements:
  * Implement a proper recusive destructor to automatically clean up heap memory upon Exit. 
  * Update the file loading loop to check 'getline' directly to prevent duplicate final line reads. 
  * Refine menu imput validation and control flow.
    
### Course Outcomes Met: 
  * Course outcome Two: Using well-founded techniques and tools in computing pratices.
  * Course outcome Four: Building secure, efficient, and maintainable software solutions (memory management and structured logic).
    
</details>
