### CSCE 315 Project 2

Term: 2021 Fall Sep. - Oct.

Contributer: 
Rong Xu(Abby): abby.xu915@gmail.com
Akash Gajendra: akash.gajendra@tamu.edu
Isaac Yeang: isaacy13@tamu.edu
Joshua Johnson: joshjoh02@email.tamu.edu
Santoshni Birlangi: santoshnibirlangi@tamu.edu

---

#### Project Mission

Our team designed a crowd-sourced recommendation system housed on Amazon Web Services (AWS) for a content streaming company that includes a database management system (DBMS) and a corresponding graphical
user interface (GUI), taking in existing watch history data to analyze trends and make personalized viewing recommendations.

#### Related Files

- database_design.pdf:

  In this file, we illustrated how we design our database including high-level and low-level designs.

- GUI-sketch.pdf:

  This is our first version of GUI sketch file.

---

#### Demo

Since connecting the AWS database need TAMU VPN request, in this case, here is a vitural demo of our project.

##### step 1: connect to TAMU VPN and make sure connect to database successfullly

![Screen Shot 2021-10-31 at 4.57.06 PM](/Users/abby/Library/Application%20Support/typora-user-images/Screen%20Shot%202021-10-31%20at%204.57.06%20PM.png)

![Screen Shot 2021-10-31 at 4.57.37 PM](/Users/abby/Library/Application%20Support/typora-user-images/Screen%20Shot%202021-10-31%20at%204.57.37%20PM.png)

##### step 2: cd to the GUI_Files folder and compile the java files to start the program

~~~sh
javac -cp ".:xchart-3.8.1.jar:postgresql-42.2.8.jar" Welcome.java
java -cp ".:xchart-3.8.1.jar:postgresql-42.2.8.jar" Welcome
~~~

![Screen Shot 2021-10-31 at 5.01.06 PM](/Users/abby/Library/Application%20Support/typora-user-images/Screen%20Shot%202021-10-31%20at%205.01.06%20PM.png)

---

##### Welcome page

![Screen Shot 2021-10-31 at 5.02.04 PM](/Users/abby/Library/Application%20Support/typora-user-images/Screen%20Shot%202021-10-31%20at%205.02.04%20PM.png)

---

##### Login page

We have two roles in this program: analyst and user. Analysts are able to have the access of users watch history and the statistics of popular trending videos. Users only have the access of their own watch history.

![Screen Shot 2021-10-31 at 5.02.31 PM](/Users/abby/Library/Application%20Support/typora-user-images/Screen%20Shot%202021-10-31%20at%205.02.31%20PM.png)

---

##### Analyst Page

(It takes a while since there is A LOT OF calculations....)

![Screen Shot 2021-10-31 at 5.10.00 PM](/Users/abby/Library/Application%20Support/typora-user-images/Screen%20Shot%202021-10-31%20at%205.10.00%20PM.png)

For the left two cols we have some charts of pop trending videos statistics. In the top right corner, the analyst can input two movies to find their connection (due to actors or directors). At the right buttom we have the hollywood pairs where shows the Top couples with highest average movie ratings which they acted together. Check hollywoodPair_SQL.pdf for related SQL commands.

---

##### User page

User has to use their User_ID to login. This page just simply lists the related user's watching information.

![Screen Shot 2021-10-31 at 5.17.47 PM](/Users/abby/Library/Application%20Support/typora-user-images/Screen%20Shot%202021-10-31%20at%205.17.47%20PM.png)
