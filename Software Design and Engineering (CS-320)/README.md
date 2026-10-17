# 3-2 Milestone Two: Software Design and Engineering

## Artifact Description
&nbsp;&nbsp;&nbsp;&nbsp;The artifact I chose was CS-320’s Software Test Automation. This is a Java-based program designed as a contact management system. This will allow users to create, read, update, and delete(CRUD) contact records. These contact records store a unique ID, first name, last name, phone number, and address. The program then validates the information that was entered to ensure it meets the specific preset requirements, such as limiting the name and address lengths. It also includes tests that will verify that the system is working correctly and rejecting invalid inputs. The artifact was created in December of 2025  for the purpose of submission to CS-320’s software test automation class as a final project. 

This project runs 3 different folders
* Contact Service:
  * Contact data classes
  * Contact service operations
  * Contact Tests
* Task Service:
  * Task data classes
  * Task service operations
  * Task tests
* Appoitment Service:
  * Appoitment data classes
  * Appointment service operations
  * Appointment tests

The tests folders contain JUinit test classes. The other folders contain the application classes.

<img width="1526" height="680" alt="Screenshot 2026-10-17 002850" src="https://github.com/user-attachments/assets/ae1bb9ba-8c0b-4dc0-aa00-1c6080aac736" />

***

<details>
<summary><h2>Running and Functions</h2> </summary>

### Project Folder

* Runs ModuleSIxProjectSnhuTompkins folder

### Installation

**Eclipse IDE for Java Developers**
* Install it using an Eclipse Installer

**Java Development Kit (JDK) 21**
* Needs Java 21 to compile proect
* The eclipse installer may bundle a JRE, but confirm Java 21 is configured in Eclipse
* A JDK is needed to compile

**JUnit 5 support**
* Needed to run the project tests
* Eclipse's Java package normally includes JUnit intergration
* If prompted select JUnit 5


### Running the Program

* Open Exlipse and locate the project in Package Explorer
* Expand a Class depening on which test the user is wanting to run
* Open the test folder (for this example I will test the ContactService class)
<br>
<br>
 <img width="259" height="220" alt="Screenshot 2026-10-17 003604" src="https://github.com/user-attachments/assets/0206a3a0-72a2-409d-ae67-5289b2469ddc" />
<br>
<br>

* Right click the Test for the class your are wanting to test (For the example this is ContactServiceTest.Java)
* Click RunAs and select JUnit Test
  * If prompted run as JUnit 5
<br>
<br>
<img width="855" height="894" alt="Screenshot 2026-10-17 003621" src="https://github.com/user-attachments/assets/528a22a3-175a-4bb4-9cbe-4bebe4db1c84" />
<b>
<br>
* View results in Eclipse JUnit Pannel
<br>
<br>
 <img width="476" height="462" alt="Screenshot 2026-10-17 003634" src="https://github.com/user-attachments/assets/cba74676-d866-491c-8dbe-adcb1142cd69" />

<br>
<br>

*A green bar shows that all test passed, If a test does not pass, it will be shown as a red error.*

  
</details>

***

<details>
<summary><h2>Enhancements and Overview</h2> </summary>
  
### Justification and Enhancement Overview
&nbsp;&nbsp;&nbsp;&nbsp;I selected this artifact because test automation is a cornerstone of computer science. IT can demonstrate an ability to both verify requirements and automate testing of the ability to verify requirements to ensure that no invalid inputs will be accepted. It also shows the ability to write maintainable, high-quality code. This project uses a structured unit testing framework to validate class requirements, boundary conditions, and input constraints. The abilities it showcases are defensive programming, testing methods, and the addition of a logic validation component. The artifact was improved in many different ways. The first major improvement is the addition of a security test. The original service test is meant for testing the functionality of the CRUD method within the application. Ensuring that an item was added or edited and can be searched. The security test is to make sure that all inputs are valid by rejecting improper IDs, no blank names, no improperly formatted phone numbers, and not allowing just anyone to edit the internal list and rejecting any operations that involve missing concatenations. I also added more commenting to ensure that the program is understandable. I also ensured that the search now returns specific criteria correctly. 
  
### Course Outcomes and Outcome Coverage plan
&nbsp;&nbsp;&nbsp;&nbsp;I feel as if I did meet the course outcomes I planned, updating my whole Java test system to include more commenting and a better understanding of security testing. I currently do not have any plans on updating my outcome-coverage plans.  I feel as if the implementation proceeded according to the scheduled code review design. By adding input validation to the contact services, it demonstrates defensive design by rejecting invalid data. I wrote more test for both balid and invalid inputs, which demonstrate that the enhancement was verfied agints its requireemnts. 

### Reflection
&nbsp;&nbsp;&nbsp;&nbsp;Enhancing the test suite reinforced how critical and thorough testing coverage is an important aspect when coming to the development of CRUD-based code. By ensuring that tests encapsulate all aspects- not just ensuring that the user input is correct, but also testing for security vulnerabilities- it allows for a quick and automated trial that can ensure that the code is working properly. The challenges I faced were how exactly I wanted to include my security tests. Originally, I wanted to add it to the previous code, but when I realized how many tests needed to be created, I added a security test branch. This also helps with the understanding and readability of the code, allowing for an overall easier experience. Otherwise, my other enhancements mostly related to ensuring proper commenting was written.

