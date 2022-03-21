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

 
