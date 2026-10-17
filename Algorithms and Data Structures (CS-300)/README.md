# 4-2 Milestone Three: Enhancement Two: Algorithms and Data Structure

## Artifact Description
&nbsp;&nbsp;&nbsp;&nbsp;This artifact is from the CS-300 Analysis and Design class; it is a binary search program created 11 months ago. The purpose of this program was to efficiently handle a large amount of data. It was designed to load classroom and student information into a database; then the user could search and print that large dataset or exit the program.

<details>
<summary><h2>Running and Functions</h2> </summary>

### Project Folder
* CS-300 Enhanced.zip
* This file is run in PowerShell

### PowerShell
* In PowerShell, type this and press Enter: .\CS-300.exe
<br>
<br>
<img width="1195" height="295" alt="Screenshot 2026-10-16 224559" src="https://github.com/user-attachments/assets/ff80b0d4-6dd7-49f8-9445-06ebbb1f8234" />

## Running The Program

First Load the courses into the program by typing **1** (An example course file is create for example purposes)
<br>
<br>
<img width="632" height="240" alt="Screenshot 2026-10-16 224855" src="https://github.com/user-attachments/assets/69e443e8-6ce3-44a3-a136-abae23326c2e" />

Next, type **2** to list the courses alphabetically.
<br>
<br>
<img width="729" height="414" alt="Screenshot 2026-10-16 224903" src="https://github.com/user-attachments/assets/411f11b9-8dbf-454f-95a0-e10e6f31b9c3" />

Type **3** to look up a course. For this example I searched course CS301. This should display the course along with its prerequisite classe.
<br>
<br>
<img width="544" height="340" alt="Screenshot 2026-10-16 224919" src="https://github.com/user-attachments/assets/b4d0e94a-7514-42cb-ba35-6b2411aecfe5" />

Finally, to exit the program type **9**

*Note: The program will pause briefly or clear the screen between actions. This is expected so the user has time to read before the cache is cleared.*

</details>

<details>
<summary><h2>Enhancements and Overview</h2> </summary>

## Justification and Enhancement Overview
&nbsp;&nbsp;&nbsp;&nbsp;The reason I selected this artifact was that it highlights my proficiency in implementing core data structures and algorithm efficiency, demonstrating my ability to transition from linear search models to a hierarchical tree structure, which is optimized for data retrieval. It also shows the ability to solve data organization and retrieval problems through the use of implemented search and pull methods within the code. For this enhancement, I improved the application by simplifying the artifact into a more readable file tree. I also improved the insertion, search, and removal of the search tree, along with adding assurances so that duplicate IDs are ignored, and the tree size count stays consistent. I improved menu input handling, adding checks for trying ot display or search before loading courses. I also added and updated the comments to help ensure clarity. Along with the improvement to the code, I also added a sample catalogue to help showcase how the project runs.

## Course Outcomes and Outcome Coverage plan
&nbsp;&nbsp;&nbsp;&nbsp;I feel as if I did meet the course outcome I planned in module one. As for updates, I added some enhancements to the code, increasing the sorting abilities of the code and overall adding some improvement to the menu handling and adding additional checks. Also by transitioning from linear storage to a biniary search tree structure, the program can automaticaly order and sort the elements upon insertion. This allows for courses to be displayed in a celan and sorted sequence. Adding these enhancements creates an overall better user experience. I also included a sorting sample to show the program's capabilities. Other than these few changes to the original plan, I also decided to leave the menu system (specifically the 1-4 and 9 to exit) alone, finding that leaving more numbers open to other commands is valuable and also prevents accidental exiting. 

## Reflection      
&nbsp;&nbsp;&nbsp;&nbsp;I feel as if enhancing this artifact gave me valuable insight into how my programming skills have improved over the course of college. When reviewing my older code, I was able to identify architectural inefficiencies and just how bad the program was originally. It was clunky, and I didn’t have a firm grasp on the code. A challenge I faced was ensuring that the proper checks went through, with the original code not catching issues such as identical inputs or the code trying to pull from a database that hasn't even been loaded. Overcoming that challenge reinforced the importance of being more detailed in my work and ensuring that all bases are covered. It also shows the importance of rigorous testing to ensure that simple mistakes, like not loading the database before searching, are caught before submission. I feel like I've come a long way compared to when I originally created this search system, and I've learned a ton about search trees. 
</details>
