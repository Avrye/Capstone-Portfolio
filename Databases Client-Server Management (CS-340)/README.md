# 5-2 Milestone Four: Enhancement Three: Databases

## Artifact Description
&nbsp;&nbsp;&nbsp;&nbsp;This artifact is CS-340 Client and Server Development, created in February 2026. This project is for a fictional client, Grazioso Salveware, an organization that trains animals. The purpose of this project is to develop a web-based dashboard using Python, MongoDB, and the Dash framework to help the staff interact with and analyze animal shelter data. I updated the code to use only a MongoDB server and Python, and to run on PowerShell. The user is able to run the command in PowerShell and view the website in the browser. 

The user is able to:
* Select a rescue category to filter the records
* The table updates with matching animals
* The pie chart updates to show breed distribution
* Click a row in the table
* The map centers on that animal’s location and shows its name and breed
<br>
<br>


<img width="1919" height="915" alt="Screenshot 2026-10-16 214145" src="https://github.com/user-attachments/assets/dfd192f3-c818-47d6-9f09-992b317a7c42" />

<details>
<summary><h2>Running and Functions</h2> </summary>

### Project Folder

* The app is in CS -340
* The main app file is run_dashboard.py
* The database connection loginc is in CRUD.py

### Installation
**Python**

* Download Python 3.10 or 3.11
* During install, check: "Add Python to PATH"
* Verify: pyton --version

**MongoDB**
This project connects to a local MongoDB database

* Install Mongo DB community Server
* Start MongoDB locally on: localhost:27017
* Make sure the database user exists with:
  * username: aacuser
  * password: SNHU1234
  * auth database: admin

This matches the code in CRUD.py
* Mongo URI: mongodb://aacuser:SNHU1234@localhost:27017/?authSource=admin
* database: AAC
* collection: animals
  
<img width="1908" height="851" alt="Screenshot 2026-10-16 223808" src="https://github.com/user-attachments/assets/100ab2d5-5a7b-4668-864b-afbff41c0f29" />


**PowerShell in the project folder**
Run: cd "C:\Users\gag48\OneDrive\Desktop\SCHOOL\CS-499\Enhancements\CS-340 run this\CS-340 Enhanced"

**Virtual envirnment**
* If it does not already exist: py -m venv .venv
* Then activate it: ..venv\Scripts\Activate.ps1

**Install the project dependencies**
* Run:
  *  python -m pip install --upgrade pip
  *  pip install dash dash-leaflet pandas plotly pymongo
  
(If the environment already includes them, this step may be unnecessary.)

**Run Dashboard**
*From the project folder: 
 *python run_dashboard.py

The user should see the output:
“Dash is running on http://127.0.0.1:8050/”

**Open the Program in Browser**
* Go to: http://127.0.0.1:8050/

<img width="1919" height="915" alt="Screenshot 2026-10-16 214145" src="https://github.com/user-attachments/assets/dfd192f3-c818-47d6-9f09-992b317a7c42" />

**Common Issues**
* MongoDB isn’t running
* Wrong username/password
* Python packages aren’t installed
* You’re not in the correct project folder


</details>

<details>
<summary><h2>Enhancements and Overview</h2> </summary>

### Justification and Enhancement Overview
I selected this artifact because databases and backend data management are foundational to modern software engineering. Showcasing an application that connects an interactive user interface directly to a live database demonstrates my ability to bridge raw data storage with practical user-facing utility. Some of the components of the artifact that showcase my skills and abilities are the use of databases such as MongoDB, along with setting up server connections and utilizing database indexes, which can optimize search queries. I also work with CRUD operations, which can create, read, update, and delete data in a database. Along with these, it also showcases the use of interactive data visualizations and UI through the building of dynamic user interfaces such as the table and map. This artifact has improved in many ways in comparison to the original. The first and most major way is the addition of a run_dashboard.py file, which allows the user to start the dashboard without using a notebook. This allows for a more streamlined startup and helps with ease of use, using a standard Dash instead of Jupyter Dash. I also improved commenting on the file to help with professionalism and readability. Also added input checks that reject any unknown fields, along with operator-style query payloads and empty update or delete filters, and fixed the original CRUD operations. 

### Course Outcomes and Outcome Coverage plan

I feel as if this enhancement has successfully met the course outcomes I established in module one across all the selected areas. First is to touch on algorithm principles and standards. By refining how queries interact with the database, such as optimizing data structures, filtering records efficiently through PyMongo, and managing the trade-offs in data storage and retrieval speed, I demonstrated the ability to design solutions that handle data efficiently. Next is computing practices and tools: through implementing CRUD operations and integrating the database backend with the application logic, I demonstrated the use of well-founded, industry- standard tools to build functional solutions. Finally, there is a security mindset. Overall, the artifact improved security by adding standard input validation and rejection, mitigating potential vulnerabilities. I did update part of my coverage plan, including the addition of a streamlined running system, completely disregarding the original way of running by including the addition of a standard dash as a way to launch the dashboard. 

### Reflection
I really struggled with modifying and enhancing this artifact. I learned that getting an application to run involves way more than just writing its code. The runtime, database, sample data, and how the interface uses that data need to work together better. One challenge was that the project notebook used Jupyter Dash, which wasn’t compatible with the environment. I added a different launcher using a standard Dash so the dashboard could run locally without having to change the original notebook. I also noted that the map didn’t function properly, so I updated it to ensure that it displayed properly. Also, to ensure that the project could run, I created a simple database to test-run the application and ensure that it displayed correctly. Overall, I learned how important it is to properly test and ensure that the program is fully functional. 


