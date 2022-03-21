# Zoom_sys
## Intro:
a project built on the linux OS
in this project we create a system simulating the Zoom system. This system has rooms and students, and the students can perform actions depending on their type.
## Students:
Every student has a first name,last name,id,average and holds all the messages recieved while the student was in the system.
There are 3 types of Students:
Diligent Student - every time the students room is working he announces that he is working.
Lazy Student - every time his room is deleted he starts crying.
Responsible Student- a Student that can send a message to all his fellow roomates.
## Rooms:
Every room has and ID and has Students in it.
There are 3 types of Rooms:
Standard Room - a Room that any student can be in.
Diligent Room- a Room that when created only diligent students can enter.
Lazy Room - a Room that when created only lazy students can enter.
A room has 2 options of splitting itself and every room can only be split once:
### Split by number of students:
the split will depend on time that the student arrived to the Room, the first half of the students that arrived will be assigned
to the left room and the second half to the right room. after the split there will be no students in the room that was split.
### Split by character of students:
2 rooms are created, a right lazy room and a left diligent room. the students are moved depending on their type and the responsible
students stay in the room that was split.
when a room is deleted all its children rooms are also deleted and all students belonging to the room or its childrens rooms will be moved to the father room. If there is no father room the student will have no Room(in the lobby).
## the System:
the System has a main menu with the following options:
1. Add Student
2. Remove Student
3. Assign Student
4. Add Room
5. Split Room
6. Remove Room
7. Work
8. Send Message
9. Print Rooms
p. Print Students
d. Print Student details
0. Exit
### System upload:
at upload time the system has no rooms, but recieves as an argument a txt file with students that will be in the system when it loads for the first time. you can see as an example the files input.txt and big_input.txt and also see the picture below. this is the only argument recieved.

![input](https://user-images.githubusercontent.com/81911093/159272653-5287c5c2-0f16-4a78-9dbd-8113788f1546.png)



### Add Student:
adding a new student to the system by recieving details:

![Screenshot 2022-03-21 131606](https://user-images.githubusercontent.com/81911093/159250584-600d4030-0790-45b0-88e5-1d601e454fc4.png)

### Remove Student:
Removing a student from the system using his id:

![remove](https://user-images.githubusercontent.com/81911093/159250990-4abaeab0-aaea-44d7-814f-94016bd9eede.png)

### Assign Student:
Assigning a student to a certain room with the student id input and room id input, if you want to move the student to the lobby
enter -1.

![assign](https://user-images.githubusercontent.com/81911093/159251266-ccd21dc2-60a7-4020-b6a8-78201d0be6df.png)

### Add Room:
the system creates a new standard room that is empty. the id of the room is the number of rooms created until the creation.

![ADd room](https://user-images.githubusercontent.com/81911093/159251801-af266347-b123-4a15-81cc-5379112a56c0.png)


### Split Room:

### Remove Room:
the system recieves a ID of the room that the user wants to remove (reminder : all lazy students will cry).

![remove room](https://user-images.githubusercontent.com/81911093/159268760-1c6b2345-1851-4547-ab9b-5f569023bc12.png)


### Work:
the system reicieves a room ID and tells all the students in that room to work, meaning all diligent students will announce that
they are working.

![work](https://user-images.githubusercontent.com/81911093/159269270-c7230363-0701-48d2-bb0f-d1a5b6e6bbda.png)


### Send Message:
the system reicieves a student ID and a message. if the student is a responsible student he will send the message to all students 
in the room.

![work](https://user-images.githubusercontent.com/81911093/159269560-5c29a731-e307-467e-924b-1df9dfb13ab0.png)


### Print Rooms:
the system prints all rooms with the following information: room id, num of students. the system prints the rooms in order of creation.

![rooms](https://user-images.githubusercontent.com/81911093/159269817-3954c829-839c-47b0-9292-a64ee1f61ceb.png)


### Print Students:
the system prints all students in the system in order of arrival.

![stud](https://user-images.githubusercontent.com/81911093/159270026-7a8923b7-3479-43da-b170-2b3fd4ad10e9.png)


### Print Student details:
the system recieves a student ID and prints his details.

![stud det](https://user-images.githubusercontent.com/81911093/159270262-8380616e-accd-4025-b376-b6b525a030a8.png)

### Exit:
the system exits.

### Error handling:
for all the functions in the main menu if the input is not valid, the system will print the error and return to the main menu.
for every error that is not an input error the system will close itself.
