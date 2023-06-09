# Critical-Path-Analysis

 Critical-Path-Analyis (CPA) is a project management tool that calculates the critical path and time required to complete the tasks of the project
and visualizes it in graphs as data structure.<br>It is developed as a part of college project for IV Semester of Computer Engineering undergraduate program.

<b> Project Memebrs</b>
+ Anil Paudel
+ [Ashim Karki](https://github.com/ashim-karki)
+ [Bishal Aryal](https://github.com/bishal0909)

### Usage

To run this program in linux, you need to install SFML first. The installation process is quite simple. The full installation guide can be found on [SFML installation](https://www.sfml-dev.org/tutorials/2.5/start-linux.php)



Clone this repository in VS code and make sure to add [MakeFile Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode.makefile-tools). 

In terminal, write `make` command. After that an executable file will be created at 'bin' . Now write `bin/main`. The program will be finally up and running.


To run this program in VS (windows) check out [Critical-Path-Analysis](https://github.com/ashim-karki/Critical-Path-Analysis)

### Program Details
+ On terminal input, we need to provide no. of vertices, their names, time durations, dependencies .
+ After successful input process, All the updated parameters of vertices, a critical path and minumum completion time will be shown along with the grpah visualisation.


### EXAMPLE

![image](https://user-images.githubusercontent.com/86644466/226087684-991da9ec-d0d1-4ba7-9a09-f5468c4b3e5f.png)
 
The dependency table of the above example is:
| Task Name  | Time  | Dependency	| Last Node (y/n)	| Task                  |
| ---------- | ----- | ----------- | --------------- | --------------------- |
| A	         | 0     |	-	         | n	              | Start
| B	         | 3     |	A	         | n	              | Creating Wireframes    
| C	         | 8     |	A	         | n	              | Designing UI                 
| D	         | 15    |	B	         | n	              | Backend Development                 
| E	         | 17    |	B, C	     | n	              | Frontend Development                 
| F	         | 12    |	D, E	     | y	              | Testing and Debugging                 
| G	         | 6     |	E	         | y	              | Content Creation and Addition
| Final Node | -     |	-	         | -	              | Demo Launch
### Input format
```
Enter the number of vertices: 7
Enter the name of the new vertex: A
Enter the time associated with the new vertex: 0
Enter the name of a dependant vertex (if any else press X to exit): X
Last node? y/n: n
Enter the name of the new vertex: B
Enter the time associated with the new vertex: 3
Enter the name of a dependant vertex (if any else press X to exit): A
Last node? y/n: n
Enter the name of a dependant vertex (if any else press X to exit):  X
Enter the name of the new vertex: C
Enter the time associated with the new vertex: 8
Enter the name of a dependant vertex (if any else press X to exit): A
Last node? y/n: n
Enter the name of a dependant vertex (if any else press X to exit):  X
Enter the name of the new vertex: D
Enter the time associated with the new vertex: 15
Enter the name of a dependant vertex (if any else press X to exit): B
Last node? y/n: n
Enter the name of a dependant vertex (if any else press X to exit):  X
Enter the name of the new vertex: E
Enter the time associated with the new vertex: 17
Enter the name of a dependant vertex (if any else press X to exit): B
Last node? y/n: n
Enter the name of a dependant vertex (if any else press X to exit):  C
Enter the name of a dependant vertex (if any else press X to exit):  X
Enter the name of the new vertex: F
Enter the time associated with the new vertex: 12
Enter the name of a dependant vertex (if any else press X to exit): D
Last node? y/n: y
Enter the name of a dependant vertex (if any else press X to exit):  E
Enter the name of a dependant vertex (if any else press X to exit):  X
Enter the name of the new vertex: G
Enter the time associated with the new vertex: 6
Enter the name of a dependant vertex (if any else press X to exit): E
Last node? y/n: y
Enter the name of a dependant vertex (if any else press X to exit):  X
```
### Resulting Graph 
![image](https://user-images.githubusercontent.com/53502633/225927409-c3e59509-604a-4969-9d90-5529e13e1109.png)
