<div align="center">
<img src="https://github.com/Anmol-Baranwal/Cool-GIFs-For-GitHub/assets/74038190/80728820-e06b-4f96-9c9e-9df46f0cc0a5" width="1000">
</div>
<br><br>

The MotorPH Automated Payroll System is an important initiative aimed at modernizing and streamlining MotorPH's payroll processes, in line with the company's growth objectives. The system prioritizes efficiency, accuracy, and legal compliance, and seeks to automate manual payroll tasks, reduce errors, and save time. It is designed to be scalable, adaptable, and secure, making it an integral part of MotorPH's organizational structure.

## Table of Contents

- [Introduction](#introduction)
  * [User Roles](#user-roles)
- [Getting Started](#getting-started)
  * [Hardware Prerequisites](#hardware-prerequisites)
  * [Software Prerequisites](#software-prerequisites)
  * [Accessing the System](#accessing-the-system)
- [User's Guide](#users-guide)
  * [Log-in (Employee's POV)](#log-in-employees-pov)
    + [Time In/Time Out](#time-intime-out)
    + [Payslip](#payslip)
    + [Leave Requests](#leave-requests)
  * [Log-in (HR head's POV)](#log-in-hr-heads-pov)
    + [Employee Management - Add Employee](#employee-management---add-employee)
    + [Employee Management - Delete Employee](#employee-management---delete-employee)
    + [Employee Management - Edit Employee](#employee-management---edit-employee)
    + [Attendance Management](#attendance-management)
    + [Leave Management](#leave-management)
  * [Log-in (Accounting head's POV)](#log-in-accounting-heads-pov)
    + [Salary Calculation and Payslip Generation](#salary-calculation-and-payslip-generation)
    + [Monthly Payroll Summary Report](#monthly-payroll-summary-report)
  * [Log-in (IT head's POV)](#log-in-it-heads-pov)
    + [Permissions Management](#permissions-management)
    + [Credentials Management - Change Password](#credentials-management---change-password)
    + [Credentials Management - Delete User](#credentials-management---delete-user)
    + [Authentication Logs](#authentication-logs)
- [Technical Information](#technical-information)
  * [Key Features and Functionalities](#key-features-and-functionalities)
  * [Use Case Diagram](#use-case-diagram)
  * [Class Diagram](#class-diagram)
- [Testing](#testing)
- [Authors (MO-IT103 - Group Carpo)](#authors-mo-it103---group-carpo)

## Introduction

MotorPH was established in 2020 and its mission is to be the first choice for Filipinos searching for competitive and affordable motorcycles. From a purely online presence, MotorPH's objective is to expand its business by opening physical stores in different parts of the Philippines. Recognizing the pivotal role of a robust employee foundation in this growth journey, MotorPH is prioritizing the modernization of its payroll system.

To support its ambitious expansion plans, MotorPH is overhauling its current payroll system, transitioning from manual processes to a streamlined and automated approach. This strategic initiative aims to accelerate payroll processes, enhance accuracy, and ensure compliance with regulations. By automating payroll tasks, MotorPH aims to minimize administrative workloads, reduce errors, and save valuable time. This not only guarantees timely and precise salary disbursements for employees but also optimizes costs, freeing up resources for MotorPH to concentrate on its core expansion priorities.

### User Roles
> - Employee - To access their payroll information and manage personal details securely.
> - HR - To manage employee information, attendance records, and leave management.
> - Payroll - To oversee payroll processing, tax calculations, and reporting. 
> - IT - To oversee system integration, maintenance, and data security.


## Getting Started

### Hardware Prerequisites
- Processor: Any modern processor capable of running Java programs.
- Memory (RAM): At least 4GB of RAM is recommended for small to medium-sized projects.
- Storage: Sufficient storage space for storing project files and dependencies.
- Network Connectivity: Required for accessing remote resources or network communication.


### Software Prerequisites
- Operating System: Compatible with various operating systems including Windows, macOS, and Linux.
- Java JDK at least JDK 19
- IDE Eclipse
- MySQL Community and Laragon

### Accessing the System

#### To access the payroll system, users need to follow these steps:

1. Install Required Software:
> - Install Eclipse IDE for Java development.
> - Install Laragon, a local development environment that includes Apache, MySQL, and PHP.
> - Install MySQL database.
> - Install Java Development Kit (JDK):
> - *Ensure JDK 19 is installed on your system. If not, download and install JDK 19 from the official Oracle website.*

2. Install Dependencies:
> - Opencsv: Download Opencsv library from https://opencsv.sourceforge.net and add it to the project's classpath.
> - MySQL Connector: Download MySQL Connector from https://dev.mysql.com/downloads/connector/j/ and add it to the project's classpath.
> - JAXB Runtime: Add JAXB Runtime dependency to the project from https://mvnrepository.com/artifact/org.glassfish.jaxb/jaxb-runtime.

3. Database Setup:
> - Use the provided dump file in the repository to set up the MySQL database.
> - Configure MySQL to use the username "root" and password "DF.w}=;$CLn+84?m]r(M%Q".

4. Start Laragon:
> - Open Laragon and start the local server. Laragon should automatically start Apache, MySQL, and other required services.

5. Import Project in Eclipse:
> - Open Eclipse IDE and import the project into your workspace.
> - Navigate to the project directory and select it for import.

6. Run Main Class:
> - In the project's src folder, locate the main class.
> - Right-click on the main class and select "Run As" > "Java Application".
> - This should direct you to the login page of the payroll system.

By following these steps, users should be able to set up and access the payroll system on their local environment using Eclipse, Laragon, and MySQL. Make sure to verify that all dependencies are correctly added and configurations are properly set up before running the application.


#### To ensure that the required dependencies are correctly added to the project's classpath, follow these steps:

1. Opencsv Dependency:
> - Opencsv library is already included in the project's classpath.
> - If any errors related to Opencsv arise, ensure that the Opencsv library JAR file is present in the project's build path.
> - To add Opencsv to the project:
> -  Download Opencsv library from https://opencsv.sourceforge.net.
> - In Eclipse, right-click on the project in the Package Explorer.
>> - Select "Build Path" > "Configure Build Path".
>> - In the Libraries tab, click on "Add External JARs...".
>> - Navigate to the downloaded Opencsv JAR file and select it.
>>- Click "Apply and Close" to save the changes.

2. MySQL Connector Dependency:
> - MySQL Connector JAR file is already included in the project's classpath.
> - If any errors related to MySQL Connector occur, ensure that the MySQL Connector JAR file is present in the project's build path.
> - To add MySQL Connector to the project:
> - Download MySQL Connector from https://dev.mysql.com/downloads/connector/j/.
> - Follow the same steps as adding Opencsv to the project's build path, as mentioned above.

3. JAXB Runtime Dependency:
> - JAXB Runtime dependency is already included in the project.
> - If any errors related to JAXB Runtime arise, ensure that the JAXB Runtime JAR file is present in the project's build path.
> - To add JAXB Runtime to the project:
> - Download JAXB Runtime dependency from https://mvnrepository.com/artifact/org.glassfish.jaxb/jaxb-runtime.
> - Follow the same steps as adding Opencsv to the project's build path, as mentioned above.

By following these steps, you can ensure that the required dependencies are correctly added to the project's classpath, which helps resolve any potential errors related to missing dependencies.


## User's Guide
This user guide serves as your comprehensive resource for the MotorPH Payroll System. Designed to empower users of all experience levels, this guide provides clear and concise instructions to navigate the system's functionalities effectively. Through this guide, you will find detailed explanations accompanied by informative screenshots. Our goal is to equip you with the necessary knowledge to fully utilize the MotorPH Payroll System's features.

We encourage you to explore this guide at your own pace, referencing specific sections as needed. Let's begin!


### Log-in (Employee's POV)
#### Step 1: Access user credentials in this [spreadsheet](https://docs.google.com/spreadsheets/d/1bLY2s66_CvoyZGd1xOYZQPb6OOt20YWh24fv9Mfqu6E/edit#gid=436645740).
#### Step 2: Log in with valid credentials.
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/5fa2b7f2-a94f-4da3-970c-a0bcdc1114c5)
*Each employee is given a unique username and password. In this example, we used the CEO's credentials.*

username: **garman** \
password: **pZ3q9fG7**

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/c5279ea7-8c26-4ad9-ba23-43ee127c747c)

*After logging in, the user is directed to the Dashboard.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/bdbdc6b8-843c-45cd-8ef1-5d7ae54e05ed)


### Time In/Time Out
#### Step 1: Time In
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/885fed19-52fc-474b-a649-b7f8da4ab1a3)
*After pressing the Time In button, the user's current status will change from OUT to IN. This will also disable the Time In button after being clicked. The timestamp and date are also recorded in the table as seen in the first row of the table.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/77853dc7-9a9c-4a81-93b7-938b90206a07)

#### Step 2: Time Out
*After pressing the Time Out button, the user's current status will change from IN to OUT. This will also disable both buttons after being clicked. The timestamp for time is recorded in the same row as the time in, as seen in the table.*
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/c7f2db68-c70e-4419-9108-662f13b1d53f)

*All records can be sorted in ascending order*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/2c4c28e1-4384-4341-bb0b-328eefa3d6bb)

*All records can be filtered and fetched by Month-Year.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/86a0cf6a-fa2c-4dfc-916a-6cd076205a1d)

### Payslip
#### Step 1: Open Payslip from the Side Bar
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/177aaba4-a18c-4e0e-bd39-62c00480a181)

#### Step 2: Select a pay period 
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/b3cffba9-872f-4060-ad0f-3375946d7f07)

#### Step 3: Export Payslip 
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/7a7be41d-3497-4249-909c-368b84a85f7d)

*After exporting the payslip, the payslip details will be saved.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/b3088b1d-cb41-435f-a36e-0c735b477a3c)

*Payslip will then be stored in your local storage.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/943f8ef5-b510-43de-951c-cf42954de6d0)

*The exported payslip:*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/2939eae8-81ca-423c-9e50-dca269e92846)


### Leave Requests
#### Step 1: View leave balances
*Upon clicking the Leave Request button, the user's leave balances can be seen at the top part of the screen.*
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/8bf2c103-ff11-40dc-961b-ad55462b087a)

*The user's leave request history can be seen at the bottom right part of the screen.*
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/033df202-c626-44f6-af9c-9a83a3753ae4)

#### Step 2: Apply for a leave
*An error will occur when the selected end date is earlier than the start date.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/7f01387c-ef12-44c4-9e97-dd7825986b48)

*An error will occur if the user selects more than the available number of leaves.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/2d69c5b4-a487-4b8a-ad8a-faa57e433550)

*Leave request with valid data input.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/f3c5cef4-e82a-4ec6-8308-e5a099666763)

*A pop-up will show the confirmation message after sending in your leave request.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/edaf8340-cce3-4569-b18d-40d81d57df1e)

*After sending in a valid request, the user's leave request history will be updated.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/06de0449-0bb4-4681-9221-131612d5d544)

*A clear button is available to reset all the data that's been placed.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/02a30e90-0d89-4349-b8f4-ebd45f092f8a)


### Log-in (HR head's POV)

username: **sanbra** \
password: **aQ2w9mE5**
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/0757766e-195a-4976-8657-f8066ac3d5a6)

*HR head's dashboard view.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/9498c422-e362-47c1-a448-7c4c4d531648)


### Employee Management - Add Employee
#### Step 1: Open Employee Management Module
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/3b8a5f9d-b5ef-49e8-8515-f81fedb8cedd)
*Default Employee Management Module view.*

#### Step 2: Press the Add Employee Button
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/d995c563-42ff-4473-826c-44291451dd6b)
*After the user presses the add employee button, a new row at the end of the table is added where the user can input details .*

#### Step 3: Input New Employee Details and Press Save Changes
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/4d3bb159-68eb-4f33-9767-2bb65d9e2010)
*System confirms the addition of the employee into the database. MySQL Database updates and adds employees to the Database**

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/1ac2753f-2970-41f7-ab8f-21d1af92005c)
*There's an issue with how Employee IDs are assigned in the application's table. When a new employee is added, the table automatically increases the ID by 1 based on the last employee shown. However, if an employee is deleted, the database remembers this and assigns the next available ID, creating a mismatch between the table and the database. For instance, if an employee with ID 35 is deleted, the table still expects the next employee to have ID 36, while the database recognizes ID 36 as available and assigns it to the next employee. This inconsistency can cause confusion and errors in the system. 
That's why, in the pictures, even though the next employee added should have been assigned ID 39 according to the table, the database records it as 41 due to the discrepancy. However, after the completed addition, the table refreshes and corrects this issue promptly by synchronizing with the database.*


### Employee Management - Delete Employee
#### Step 1: Select the row of the employee to be deleted
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/744cf64b-bd13-4cbf-a290-5d23b3607515)
*Suppose we wrongly made an entry like this one.**

#### Step 2: Employee Deletion Verification
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/51481089-31e9-4f32-b905-f5ec06ad375e)
*The system implements a double-check mechanism when deleting an employee.*

#### Step 3: Employee Deletion Confirmation
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/9f03942a-be48-4fcb-9724-bf529836f538)
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/7abc963e-f575-423a-b7b9-3c27a0d89116)
*The employee with emp id 38 is deleted from the database.*


### Employee Management - Edit Employee
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/26df1854-1923-40f8-841d-5f318d248956)

*Default view of the edit employee window.*

#### Step 1: Select Employee to edit details from the dropdown
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/1d32efc6-2265-4600-a764-4cff6de17a59)

#### Step 2: Type the information detail change you wish to change in the textbox.

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/9dbe192e-d94d-4815-b3c4-bfb47af29e9a)

*In this example, we are going to edit Manuel III Garcia's last name to Santos.*

#### Step 3: Press Save Changes and Saved Changes Confirmation
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/1c69e907-0eb4-458d-8517-2c8671e9ebf0)
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/58b67c56-443c-4771-b775-247d95b5a8eb)
*The change in last name to Santos is also reflected in the database.*


### Attendance Management 
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/2c1ee90e-248f-49c4-a5c1-d3c6a2940e2e)

*Default view of the attendance management window.*

Records can be filtered by Year-Month.
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/ef88107c-50b0-4976-bbb6-81fea4194388)
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/af24cc1d-2074-4f53-8eb1-720e8719e8e1)

*Records filtered by 2023-02 or February 2023.*

You can also search for an employee. The search bar accepts both Employee Name and number.

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/5147d70a-4d72-45c2-b894-829d670ff68a)

*When searching for 'Santos,' both 'Delos Santos' and 'Santos' appear due to the search algorithm including partial matches. This means that names containing 'Santos' in any part of the string will be included in the search results.*
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/c55c0c25-f3f5-42a7-86ea-e5cdaeb6469c)
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/9fb94e77-d5df-4712-bf25-0c937e9958c8)



### Leave Management 
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/91770cc1-2163-46fc-b19f-74546564c57d)

*Default view of the leave management window. The first table shows the Leave Requests while the second table shows the Employees' Leave Balances.*

#### Step 1: Select a Leave Application
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/7ac4477d-7ca1-42a8-8980-f21ffc20ee8b)

#### Step 2: Press Approve
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/85b0d8d0-3dcd-4ac4-887d-9aea0e73e057)

*In this example we are going to show how the leave approval works.*

#### Step 3: After pressing Approve, Pop up Confirms Leave Approval  
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/4009733d-df18-487b-bdce-1d952545b921)

*Table also updates the Leave Application from pending to Approved.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/dcd7683f-a660-484e-97b6-8e982e1f796d)

*Leave Balance also updates to reflect the approved day/s.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/33de521a-c2d5-4cb8-9bb2-c9689db555fe)

*Leave Log in the database also updates to reflect the change.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/98f975a8-baab-49c8-a5eb-2c8eed71243a)

*Leave Balance in the database also updates to reflect the change.*

Exception handling: If a Leave has already been Approved or Rejected, it cannot be changed again.
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/1c21b105-bca7-46b8-a7de-57ccb7319c46)
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/9c52109e-c982-4c6e-aad7-0a7fb85128fe)



### Log-in (Accounting head's POV)

username: **alvrod** \
password: **yH6t3eS7**
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/e94dfb6e-3e0f-4fb0-9f41-53cfc425fb48)

*Accounting head's dashboard view.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/21487448-a8a2-4dde-9d9d-547176282c4c)


### Salary Calculation and Payslip Generation
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/b21c01af-6c55-46b4-b5b5-2aa080d5dce2)
*Default view of the Salary Calculation window.*

#### Step 1: Select a Pay Period
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/aa90f0ec-ce30-4495-9bd4-838c96189c1c)

*If records already exist it displays the information in the tables.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/4f29dfa2-e952-40a3-8c46-59b69396d8c5)

*If records don't exist yet it displays shows no records in the Employee Months Worked Table.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/f7fb09f1-c191-4ce4-9b6f-40dad0884577)

*As can be seen here in the database, there are no records yet for 2023-04.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/91ffe7da-13d5-4a8b-ac35-e3665229c94e)

#### Step 2: Press Calculate Monthly Hours Worked
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/997f5ec8-b8b1-4811-8792-d8476a7b0f7d)

*The system verifies the calculation of monthly hours, confirming the recording of payslips. It's important to note that each payslip is added individually to the database, which may take some time for confirmation.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/8beea42b-a82d-481b-b9dd-06bda0366288)
*Database now has records for 2023-04.*
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/cc17281d-118c-41b9-82fd-ecbf8ebcef3f)

*Table inside the window also updates to show records*

#### Step 2: Select Employee from the Table
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/5af23006-a4a5-445b-8052-afd5c512819b)

#### Step 3: Press Generate Payslip
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/930ba5b4-9f76-419c-a3d5-9baeb7c4df1a)
*The payslip details are displayed and automatically populate the text boxes with accurate information.*

#### Step 4: Export Payslip
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/c15b35c7-e80f-4e44-9a76-01e2c67b0344

*After clicking "Export," a popup box will appear, allowing you to choose the location on your local computer where you want to save the file, and prompting you to enter the desired file name.*

#### Step 5: Write Filename and Press Save
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/a7da15ca-748e-4407-a0d0-04251c842458)
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/f914848e-de22-4a1a-8099-187581c1553b)

#### Step 6: Open the payslip.txt file
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/551a4d6f-6511-41fb-b37b-bdff429a5cfc)

*Find the file in the location where you saved it.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/94d4a1d8-f473-4b4b-8444-8e969f633abe)


### Monthly Payroll Summary Report
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/c33d3684-f6c6-4df4-a487-eaae4b01bc45)

#### Step 1: Select a Pay Period
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/076cd652-3471-4398-92aa-6415dc887d8f)

*The report for the selected pay period is shown in the table.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/6cf2543f-af3f-4956-8802-b0f612999403)

*A summary of the report can be seen at the bottom.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/00800e30-cfb5-445d-8f10-584de4ecca7e)

#### Step 2: Export the payroll summary report
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/142f7484-41b3-4e44-8387-4cb28be78a06)

*Rename the CSV file.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/f5255fdc-7ae8-4024-8d7a-8efcc9eb6d24)

*A pop-up will display after successfully exporting the summary report.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/c5018791-36a5-474b-a4b1-5dd961af7762)

*The exported summary report will then be saved to your Documents.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/2fa9b95a-a44a-4147-b1f7-6f82022fb35a)

#### Step 3: Open the CSV file
*This is what the monthly payroll summary report file would look like after opening it.*
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/fdf5902a-19b8-49a1-b46b-c2f33dd99334)


### Log-in (IT head's POV)

username: **heredu** \
password: **dG7s3eQ2**
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/8e8dba1f-7b09-4c36-9d0e-1d79f2b9169a)

*IT head's dashboard view.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/c64d5c17-8396-4964-8141-94463285ede6)

### Permissions Management
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/616fb5b5-f76c-4be3-82d1-fad60217fde0)

#### Step 1: Select Employee to show permissions
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/5353f947-d7e5-4153-982b-de0e7ba05e5d)

*Default view of the permissions management window. The first table shows the Employees and the 2nd Table shows the permission granted to a selected employee.*

#### Step 2: Grant access to the selected employee
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/546d9221-9066-433f-a5b6-072ef5cb119d)

*After granting permission to the chosen employee, the button for that function will now appear on their dashboard view.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/301a8622-cf8a-4d87-8152-73bf254fb914)

*HR permissions.*

![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/80d08042-b7f9-4055-be22-570f1a6a66ec)

*Payroll permissions.*

![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/124635709/9e46175c-1b45-449a-acfb-1436249cdb71)

*IT permissions.*

![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/124635709/225465fb-8cd4-4fee-b732-7fe1d54b91e6)


### Credentials Management - Change Password
*Here, the IT head can reset employee's passwords.*
![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/124635709/a7d63868-fa9b-4591-9892-37b85318befa)

#### Step 1: Select the employee whose password you'd like to change.
![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/124635709/6c354dbd-00ac-45a8-9a93-018d86518067)

#### Step 2: Change the password for the selected user.
![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/124635709/1ef0d518-d156-42d5-b024-5145bd91c83e)

*The system confirms that the password for the user was changed.*
![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/124635709/58110223-ec1e-4996-a47d-8e52556c5aa6)

*When changing a password, the system securely updates the saved password in the database using SHA-256 encryption. SHA-256 is a cryptographic hash function that converts input data into a fixed-size string of characters, ensuring data integrity and security. This encryption method is widely used in computer security applications due to its strong cryptographic properties.*

### Credentials Management - Delete User
![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/125028278/30ed3da6-edca-472e-bd47-b7ed7b345c77)

#### Step 1: Select a user to delete
*View before deletion.*
![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/124635709/c08de654-c4ff-4faf-b730-14e517d7ff34)

*Selected user*

![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/125028278/fe8c500a-fe76-4c74-a868-d9fbeea00584)

*Selected user to be deleted from the database*

![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/125028278/27788d26-a9cc-4be2-a2ec-5853b1fe0bb8)

#### Step 2: Delete the selected user
*A pop-up will show after successfully deleting the user.*
![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/125028278/4a93c05e-a382-4d97-b121-0d7592fb2ad3)

*User is now successfully deleted in the database.*

![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/125028278/ce69a023-2f00-4b17-b8dc-7a64d4beeed3)

### Authentication Logs

#### Step 1: View authentication logs
![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/125028278/32378986-297e-4e83-88b8-38d24eb0a5e8)

#### Step 2: Sort authentication logs
*The authentication logs can be sorted in ascending or descending timestamps order.*
![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/125028278/713ea207-6ee7-4c0b-b796-23ea49b0973f)

*The system records unsuccessful logins as '0' for employee ID.*

![image](https://github.com/shaneabrasaldo/MotorPH-Payroll-System/assets/125028278/dc2735a5-eeb1-48af-a504-db89083db280)



## Technical Information

### Key Features and Functionalities
<p>The key features and functionalities of MotorPH's proposed payroll technology solution encompass a comprehensive set of tools and capabilities designed to streamline payroll processes, enhance accuracy, ensure compliance, and empower employees through self-service functionalities.</p>

#### Account Login
> The payroll system incorporates a secure login process, ensuring personalized access for employees and safeguarding sensitive payroll data.

#### Employee Information Management
> A centralized database maintains comprehensive employee information, including personal details, salary structure, tax information, and relevant documents, ensuring data accuracy and accessibility.

#### Time and Attendance Tracking
> Integration with a time and attendance system accurately records employees' clock-in and clock-out times, securely storing this information for efficient tracking of work hours.

#### Salary Calculation
> Automated salary calculations based on work hours, overtime, bonuses, deductions, and taxes ensure compliance with local laws and regulations, minimizing errors and optimizing payroll accuracy.

#### Employee Self-Service Portal
> A secure portal lets employees conveniently access their personal and payroll details, empowering them to apply for leave, record time in and out, and view personal attendance information. This self-service functionality enhances employee satisfaction and reduces administrative burden.

#### User Role Specification
> <p>Implementation of various user roles and permissions ensures granular control over data access and maintains data security within the system.</p>

#### Employee Leave Management
> Employees can easily apply for leave and view their leave balance, while HR administrators can track and manage leave requests and balances efficiently, ensuring smooth leave management processes.

#### Report Generation
> The payroll system generates individual payslips with employee-specific salary details and deductions. Additionally, monthly summary reports compile key metrics such as total wages paid and taxes withheld for the entire workforce, facilitating informed decision-making and regulatory compliance.


## Use Case Diagram
![image](https://github.com/shaneabrasaldo/Java-Calculator/assets/125028278/c9c1a96a-2a96-4847-964d-eef075c71b94)

The MotorPH Payroll System operates on a modular architecture, featuring interconnected components that facilitate seamless data flow and task execution. This system accommodates four primary users: Employee, HR, Payroll, and IT, each with specific roles and functionalities. The use-case scenarios illustrate how the system facilitates interactions between users and the platform to achieve defined objectives. The login scenario allows users to access the system securely. For HR and Employee users, viewing and managing employee information are crucial functionalities, enabling them to access detailed records and make necessary updates. HR personnel can add, edit, or delete employee records, ensuring the database remains up-to-date. Employees can also access their information for reference, fostering transparency and accountability. Leave management functionalities, including requesting leave, checking balances, and approving or denying requests, streamline the process for both HR and employees, promoting efficient time-off management. Time and attendance tracking functionalities enable employees to record their work hours accurately, while HR can monitor attendance records for administrative purposes. The payroll administration functionalities encompass processing payroll, editing payroll data, generating payslips, and managing user roles and permissions. These features empower Payroll administrators to ensure timely and accurate salary payments while enabling IT administrators to maintain system security and user access control. Overall, the MotorPH Payroll System enhances operational efficiency, accuracy, and compliance, contributing to improve employee satisfaction and organizational productivity.


## Class Diagram
![ERD - Class Diagram (2)](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/deab9e61-2148-4556-9d15-aafebc909caf)

The class diagram illustrates the structure of MotorPH's payroll system, with related classes visually highlighted to indicate their connections within the module. Each colored area represents a specific module or functionality, such as account login, employee information management, time and attendance tracking, salary calculation, employee self-service portal, user role specification, employee leave management, and report generation. By visually distinguishing related classes, the diagram provides a clear overview of how different components of the system interact and contribute to its overall functionality.

![ERD - Class Diagram (3)](https://github.com/shaneabrasaldo/Java-Calculator/assets/124635709/4cb219e0-5a16-432f-a7ca-abfe907d56e7)

## Testing
[Test Cases and Issues](https://docs.google.com/spreadsheets/d/1IdAsLesw17KgByksMrziTsWmAmPS_WMahOdPHjtlP5M/edit?usp=sharing)

## Authors (MO-IT103 - Group Carpo)
<div>
  <div>
    <img src="https://user-images.githubusercontent.com/74038190/216655825-c639587f-6eb0-4841-b622-9f522f55d40e.gif" width="120" />
    <p>Zyra Camille Hachero</p>
  </div>
  <div>
    <img src="https://user-images.githubusercontent.com/74038190/216656971-9a208a88-e6ad-4b7a-88eb-c410e4cf0e00.gif" width="120" />
    <p>Shane Mishael Abrasaldo</p>
  </div>
  <div>
    <img src="https://user-images.githubusercontent.com/74038190/216656977-ef584e23-480a-4d1c-8c3f-7d045910ddc9.gif" width="120" />
    <p>Jogine Novillas</p>
  </div>
</div>


