# Student-Hub

In the present world of networking, people connect with one another from the nook and corner of 
the world. When it comes to student connections, it is essential for all the students to have a 
database accessible about the details of fellow students in their class to connect. There are few 
opportunities for overseas students at a university like Northeastern to meet classmates who will 
enroll in the same course or intake as them and form professional connections rather than 
connections on social media. In order to overcome this, our project “Northeastern Student Hub“
will help in connecting students from various colleges such as CPS, COE, KHOURY, and streams 
under one roof with the required data. From this data, a student can find his/her roommates and 
students of similar interests. This will help students connect with genuine students and not get 
scammed or dragged into third-party sources that collect potential student data.

**Business Problem**

Our project aims to create a holistic system for students who aspire to study abroad. The project's 
primary goal is to provide a student database that will help students access their peers who have 
applied to a particular university and their background, which includes their priorities. This system 
will largely help international students as most of them suffer due to the lack of a proper channel
with legitimate information. This system will help students be connected well before their college 
start date which in a way helps students act like a bridge before they even meet in person.

**EER MODEL**

![image](https://user-images.githubusercontent.com/66838658/208557684-91098e58-f27d-491e-af40-b231ada73e9e.png)

**UML Diagram**

![image](https://user-images.githubusercontent.com/66838658/208557744-b3d5b66d-84da-4c80-95dc-ba0ebc8f9670.png)

** Relational Model** 

Student (Studentid, Name, Ph_no, Email, dateofbirth, gender)
Application_details (App_id, Stud_id, College_id, departmentid, status)
University_and_college (College_id, college_name, campus, email)
Department (Department_id, College_id, Depart_name, email)
Offers(departmentid, courseid)
Course (Course_id, Course_name, Professor_id)
Class_room (CRN_NO, course_id, studentid, Classschedule, Class_type, groupname)
Professor (Professor_id, Professor_name, email, Office_hours)
Teaching_assistant(taid, taname, email, officehours)
Sends(studentid, message_id)
Stores(crnno, message_id)
Message (message_id, content, Message_time, conversation_id)
Housing_and_food(Stud_id, House_type, Food_choice, rent_preference, Zipcode_preference)

