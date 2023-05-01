Download Link: https://assignmentchef.com/product/solved-bbm-203-assignment-3-linked-list
<br>
Subject of this experiment is usage of linked lists. A linked list is a linear data structure, in which the elements are not stored at contiguous memory locations. The elements in a linked list are linked using pointers as shown in the Figure 1.

Figure 1: Representation of single linked list

In simple words, a linked list consists of nodes where each node contains a data field and a reference(link) to the next node in the list.

In a single linked list, every node has link to its next node in the sequence. So, we can traverse from one node to other node only in one direction and we can not traverse back. We can solve this kind of problem by using double linked list.

Double linked list is a sequence of elements in which every element has links to its previous element and next element in the sequence. In double linked list, every node has link to its previous node and next node. So, we can traverse forward by using next field and can traverse backward by using previous field. Every node in a double linked list contains three fields and they are shown in the Figure 2.

Figure 2: Representation of double linked list

Page 1 of 5

<h1>1           Problem Definition</h1>

In this assignment, you will have input.txt which has footballer’s information on each line about a football league. In each row,there are the name of the footballer, the team name of footballer who scored, the name of the away team, minute of the scored goal and the match ID. Each line is read and parsed one by one, you need to create your linked lists according to this information and add the data you have read from the file to the linked list by the adding method. The point to note is that the information can be mixed. The linked list structure you will build is designed as follows.

Figure 3: Linked List Structure

As shown in Figure 3, each node should contain footballer’s name, team name, pointer which points to the another linked list and one pointer. The last pointer always points to the next member of the list. If the pointer is NULL, then it is the last node in the list. In the second linked list, there are away team name, minute of goal scored, match ID and two pointer. This pointer also shows the next node as it is in the other linked list.

<h1>2           Experiment</h1>

In this experiment, you are supposed to develop a simple search engine that uses linked list mentioned above. Firstly, you will read input.txt file and create linked list according to the ascending order of the names of the footballers. The information of football players in the file are not sequential. So you should make a ranking according to the name of the footballer while you are creating the linked list. The input.txt is shown and detailed in next section. Using these linked lists, write the C++ program that makes the following calculations.

<ol>

 <li>The period in which the most goals are scored in the league (0-45 minutes in the first half, 46-90 minutes in the second half). If the first half, print 0. Otherwise, print 1.</li>

 <li>Find the top goal scorer and print his name on the screen. There is no player who scored his own goal. (There may be more than one footballer with the same goal count, in this case all should be printed.)</li>

 <li>To print the names of footballers who scored hat-trick. (Hat-trick is the scoring of three and more goals in a game by one player)</li>

 <li>Print the team list in the league</li>

 <li>Print the list of footballers</li>

 <li>Matches and goals of given footballer</li>

 <li>Sort by match ID in ascending order of given footballer</li>

 <li>Sort by match ID in descending order of given footballer</li>

</ol>

You should use the linked list that you created for the above operations. In the final homework, all these operations should be listed on the output.txt.

<h1>3           Execution</h1>

The name of the compiled executable program should be “assignment3.cpp”. Your program should read input/output file names from the command line, so it will be executed as follows:

You will be given sample input and output files. You can get these files from piazza. Different input files will be used when evaluating the assignment. So it is recommended that you test your program on sample input and output files. The program must run on DEV(dev.cs.hacettepe.edu.tr) UNIX machines.

<h1>4           Input and Output</h1>

You will have two input files which are input.txt and operations.txt and one output files in this assignment. Input file is shown in Figure 4. As shown in Figure 4, each line has a footballer information. The data in each line is separated by commas. You should read and split the data by comma and add it to the linked list. Parameters for items 6, 7 and 8 are given in the

Figure 4: input.txt

operations.txt file. In operations.txt, each line corresponds to one item. And each line has two parameters separated by commas. As shown in Figure 5, there are three line for sixth, seventh and eighth item. For example, for the sixth item you should print matches and goals of Diego Costa and Karim Benzema. You should do similar operations for seventh and eighth items. As output, you should print all the items mentioned above output.txt file.

Figure 5: operations.txt

Your program should write outputs to the output.txt file. Your output should be as shown in Figure 6. Your outputs will be evaluated automatically. So you should create your outputs by taking this format into consideration. As shown in 6, you must have results in a bottom line of each item definition. Results for items 6, 7 and 8 should be splitted by commas.