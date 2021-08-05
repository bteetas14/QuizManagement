1. Introduction   
   
1.1 Purpose   
Online quiz management system is a software which is very helpful in current times when education is delivered through online channel. This software will reduce the complexity of taking tests online.   
a.	It saves time as several students can together give a particular exam.   
b.	The system automatically calculates the result, thus reducing the manual task of evaluator and results are available to students in no time.   
c.	Administrator can add/modify/delete questions.   
d.	Users must register, and they can give test with their ID, thus enabling authenticity.   
   
1.2 Document Conventions   
The following conventions are used throughout the SRS document:   
a.	Administrator - A user with administration privileges of the software   
b.	User - A general user of the software   
c.	Client - Target users of the software, students/applicant in this case   
d.	Examiner - Checks the answer of tests and gives the result.   
   
1.3 Intended Audience   
The main target audience for the software is the educational institutions which include the schools and colleges as well. It also includes corporates and MSME’s intending to take surveys and customer feedback.   
   
1.4 Scope   
Scope of this software is very broad. It can be used in –  
a.	Conducting online exams in institutions   
b.	Conducting quiz & survey in corporate   
c.	It can be accessed remotely at any location & at any time.   
d.	Physical examiner need not be present   
 
2. Overall Description   
2.1 Product Perspective   
  Since this is at initial stage so, there is no cost for because this new idea to enhance the educational system.   
          
  So, the source code is made free for all. There are various reasons why should anyone use this program. First, it is a framework where you can create edit and store multiple choice questions.   
         
  Second is an easy and reliable testing program that is unique in its category where you can use the questions you have created in a way that represents test sessions. And third due to its open-source nature you can modify it according to your needs.   
   
The Quiz Management System is an online exam cum survey platform. The process includes mainly 3 steps -   
   
a.	Login   
The user has to login to their account when they first enter the site.    
   
b.	Test   
It is the most important page of the system. It includes:   
i.	Subject page to select the subject to give the exam.   
ii.	After starting the test, the timer starts according to the allotted time. It has the option to skip, answer and flag the questions. It also shows the total answered and unanswered questions. Grid form is also available where user can go to any question without hassle.   
   
2.2 Product Functions   
There are 2 types of users –    
   
a.	Administrator/examiner   
They have rights to do the following i. Create/delete user account  
ii. 	Change password  iii. 	Can access any user account  iv.       Check the result/scores  v. 	Modify/edit scores   
   
b.	Student/user account   
i.   	View tests available to them  ii.   	View their test marks   
   
2.3 User Classes and Characteristics   
There will be 2 kinds of users that will visit the product for different reasons.   
Physical actors:   
a.	The administrator/examiner will visit for admin privileges mentioned in 2.2 a. and for the loading the test paper.   
b.	The student/user account will visit to appear for the test and to check their marks.   
    
System actors:   
a.	Client: The client is the system that connects to the server and handles the tests based on the session and finally submits the information back to the server.   
b.	Server: The server is the system that accepts multiple connections from clients and saves the results.   
c.	Database Editor: The database editor handles all the question tools used to construct modify and save questions and make different tests for the students. Also, it is responsible for logging the session info and restores them for better study. The primary actor is the client that connects to the server and takes the test. The term student is to be used as a physical actor to describe the physical user of the client. The same term is used for the teacher who is the physical user of the database editor and server and is responsible for the good behaviour of the system and to make sure everything goes well.   
   
2.4 Operating Environment   
This product will work in almost all web browsers. The only basic requirement is an internet connection.   
   
2.5 Design & Implementation Constraints   
•	MS SQL server will be used as SQL engine and database.   
•	Users may access from any computer that has Internet browsing capabilities and an Internet connection.   
•	Users must have their correct usernames and passwords to enter their online accounts and do actions.   
   
2.6 Assumption and Dependencies   
We assume all users have basic computer operating knowledge and our quiz system has a very interactive and user-friendly interface.   
For creating the windows forms and setting up the core program my tools were used so far that effect overall rhythm of software here for better understanding the know-what to do rather than the know-how to do it we assume that the reader is not interested in knowing how to create and design windows forms and how the program is coded at that time.   
   
2.7 User Documentation   
The manual provided will guide the respective user through the product like technical details etc.   
 
3. System Features  
3.1 Database   
3.1.1 Description   
This database is supposed to store, retrieve, update, or edit information related to –    
•	Profile of both types of users   
•	Student/admin details   
•	Test results   
   
3.1.2 Response requests   
For Administrator - The admin will login and the credentials will be verified. If credentials are valid, the admin will be able to perform the tasks like add/delete student record, add exam details etc.   
   
For user/student - The student will be given login credentials though which they can login. From the menu they can appear for tests, view scores, or view their profile.   
   
3.2 Functional Requirements   
Functional requirements the services provided to user by the product.   
There are 2 subdivisions in the type of user.   
•	Administrator – The admin keeps track of the tests and scores and creates/modifies the student account as per requirement.   
•	Candidate – The candidate will login and take the test as assigned. The results will be displayed after completion of test.   
   
 3.2.1 Perform Validation   
   
Input:   
Input   	Unit   	Range   
Username   	Character   	3-10   
Password   	Character   	6-15   
   
Output:   
User will go to homepage.    

3.2.2 Conduct Test   
   
Input:   
Input   	Unit   	Range   
Question   	Integer   	1-99   
Answer   	Character   	A-D or A-E   
    
Output:   
After successful evaluation & validation in the backend, the result will be displayed.   
 
4. Non-Functional Requirements   
4.1 Performance Requirements   
Some performance requirements identified is listed below:   
•	The database shall be able to accommodate a minimum of 10,000 records of students.   
•	The software shall support use of multiple users at a time.   
•	There are no other specific performance requirements that will affect development.   
   
4.2 Safety Requirements   
The database may get crashed at any certain time sue to virus or operating system failure. Therefore, it is required to take the database backup.   
   
4.3 Security Requirements   
Some of the factors that are identified to protect the software from accidental or malicious access, use, modification, destruction, or disclosure are described below. Keeps specific log or history data sets.   
•	Assign certain functions to different modules.   
•	Restrict communications between some areas of the program.   
•	Check data integrity for critical variables.   
•	Later version of the software will incorporate encryption techniques in the user/license authentication process.   
                     
  Communication needs to be restricted when the application is validating                    the user or license (i.e., using https).   
 
5. Other Non-Functional Requirements   
   
5.1 Performance Requirements   
Checking the fact that a system must perform as what every user expects.   
So, in every action – response of the system, there are no immediate delays. In case of opening window forms, of popping error messages and saving the settings or sessions. Also, when connecting to the server the delay is based on the distance of the 2 systems and the configuration between them so there is high probability that there will be or not a successful connection in less than 20 seconds.   
   
5.2 Security Requirements   
This program uses object-oriented mechanisms to protect its data passed using methods also there is not currently a security schema of this program. Thus, the log files that are being created are readable using a simple text reader.   
   
5.3 Software Quality Attributes   
   
5.3.1 Availability   
Checking that the system always has something to function and always pop-up error messages in case of component failure. In that case the error messages appear when something goes wrong so to prevail availability problems.   
   
5.3.2 Usability   
Checking that the system is easy to handle and navigates in the most expected way with no delays. In that case the system program reacts accordingly and transverses quickly between its states.   
   
5.3.3 Functionality   
Checking that the system provides the right tools for editing question databases, creating session tests, and analysing the test sessions. In that case the tools.   
             
6.  Hardware and software Requirements   
   
6.1 Hardware Requirements   
•	Systems having processors minimum 2.8.   
•	Printers may laser etc.   
   
6.2 Software requirements   
•	Microsoft windows all versions, Linux, Mac, Solaris, Ubuntu etc.   
•	Java   
•	Database with DBMS (database management system) tools as per requirements.   

7.  Future scope and conclusion   
  
7.1   Future scope   
Technological advancements in this era of digitization along with being a boon to the world have been advantageous to the educational sector too. The introduction of online exam system replaced the conventional system of assessment.   
Before proceeding further let us understand the concept of online examination software. Exam software allows users to take online tests and automatically generate results based on the answers marked by the users.   
•	Safe and secure data:   
Various tools offered by exam software have enabled the assessment conducting agencies to manage the crucial data related to examination questions and test-takers safely.   
•	Reduce administrative burden:   
Organizing and running exams online not only reduces an organization’s administrative burden but also saves cost and time. Online quiz management with its objective to make evaluation massive but simple, cost-effective, and faster has replaced the pen paper-based assessment.   
                     
i.	As is the case with all the applications, we will try to make this more user friendly.  
ii.	Captcha verification can be added at login page.  
iii.	We can add a search option for the admin to easily view, edit, delete questions  
iv.	The option to download the results in .pdf/.csv/.xlsx can be added.  
v.	The option of switching and attempting any question at any time can be added.  
  
 
7.2    Project Outcomes  
With the help of this project, we were able to learn the following concepts: 
i.  	JavaFX – It is one of the very important features with which we can enhance the Graphical User Interface (GUI) which in turn improves the user experience.  
ii. 	Classes & Constructors – it is widely used in the project  iii. 	Inheritance – Many of the code blocks need to be inherited to avoid long lines of code. It turns out to be very useful  
iv. 	SQL – it is a very important feature, which helps us to store data and  conduct a quiz. The questions, login credentials, result etc. can be 
accessed and verified using SQL.  
 
7.3    References https://www.javatpoint.com/exception-handling-in-java https://stackoverflow.com/questions/27679867/jtable-how-to-use-
rs2xml/27680067 
https://www.youtube.com/ 
https://docs.oracle.com/javase/7/docs/api/javax/swing/JFrame.html 
 
7.4    Conclusion   

The whole project is designed in such a way that future improvements are easy to implement. We can conclude that:  
i. 	Only authorized users get access to the admin functionalities. 
ii. 	Updating information is easier  
iii.  	Conducting a quiz through a software improves the efficiency and ease with which we can conduct a quiz.  
        Online Quiz Management System is significantly superior among the other exams. We have come to result that the problems can be solved by introducing new security systems using biometrics, we can identify the student’s identity by analysing digital signature or by fingerprint mechanism and by providing web cameras in the examination hall. Although web cameras sometimes get failed. We conclude that no mechanism is ideal. Each mechanism has some restriction on its own. Key concepts are to develop paperless environment and to convert all the documentation in digital form.   
  

    
 

   
