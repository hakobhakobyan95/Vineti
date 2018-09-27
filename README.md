1.What teams at Vineti are you interested in and why?(Dev or QA)

I intersted in QA becouse for me QA testing is challenging and very satisfactory. But also intersed and in DEV.

2.What is your favorite programming language and why?

My favorite programming language is JavaScript. JavaScript is the only language that can be used for true full-stack web development in major browsers. JavaScript has the largest ecosystem of wonderful tools, libraries, and frameworks that are used by both small and big teams. JavaScript code can be tested in the browser without any setup. Nearly every programmer on Earth knows a thing or two about JavaScript making it easy to find help.

3.What is a linked list?

Linked list is data container like a vector array. If in array the elements saving on memory in next bits then in Linked list the elements
can saving on any places in memory but every member of list have pointer to his next and previous member. Linked list using when need to have 1000
elements but we didn`t have any  1000 free nexting bits but we have 1000 bits in memory.
In linked list the push element is quickly but searching time is slowly.

4.You work in an ice cream shop and step into the back for a few minutes.You returs and see a large group of people waiting.How would you serve them?

I would serve the people based on first-come first served basis.(it like a queue FIFO first input first output)

5.How would you test a pen?

Test the fallouns poats:

-writing or not

-is the color as to be

-is the thickness appropriate

-close it write on surfaces,which are required

-to test writer it writes the specified length,will write it for some length and check the used amount of.Then the result will extrapolate to find it .

6.As a test engineer in Amazon what would tou test firs (assumnig authentication functionality is already covered)?

If the buy button works because it is very important function.Also can testing and back button and Logout button.

7.You have a list of numbers from one to one million and there is a missing number.How would you find the missing number?

At first I’ll calculate the sum of lists elemetns,then the sum of 1 to N nubmbers.The difference thus two numbers will be the missing number.

8.How would you determine the angle between the hour-hand and minute-hand of clock at 3.20?

3.20 means the hour hand is 1/3 pasts from 3,and the minute hand is on 4.The angle between 3 and 4 is 360/12 = 30.Subtructing the 1/3 from 30,will be 20.

9.How would you determine if a number is a power of two?

Will calculate lossN.If the result is integers,then the N is power of 2.

10.How would you remove duplicates from list?

Will create a new list and write the number in it if the new list dosen’t contain it yet. Can and sort the list and check: if there are numbers after each other that are equal, if equal remove from list.

11.How would you determine if a string has all unique characters?

First will divide the string to symbols and if a symbol is not equal to a space, then will push to the list. After them sort the list and check: if there are numbers after each other that are equal, then there are repetitions, otherwise: the all string elements are unique.

12.How would you reverse a string?

This is my simple code in JS which is reversing given string

for(var I = 0; i < (str.length/2);i++)

{
var temp = str[i];
str[i] = str[str.length-1-i];
str[str.length-1-i] = temp;

}

13.How would you compress a string such that ‘AAABCCDDDD’ becomes ‘A3BC2D4’? Only compress the string if it saves space

I will count the number of successive characters one after another. When the current character is not equal to the previous one, I will store the number of repetition time of previous character and start to count the new one. The process continues till I have not reached the last one. If the number is greater than 1, I will type the character and the number, otherwise I just write the character only. If there are more than 2 numbers in the newly received line then I will return the received string.

14.Given an array of 0’s and 1’s, how would you move all of the 0’s to the beginning of the array and all of the 1’s to the end of the array?

I will count the number of 0-s (N0) and 1-s (N1) that appear in the string, and create a new line with N0 zeroes and N1 ones. Example if the string is 011000110 the number 0s is 5 and the number 1s is 4.The new line will have five zeroes and four ones.(000001111).

15.How would you design a vending machine or a toaster?

To design a vending machine we need some specifications:

- what coins and bills it accepts, 

- what is the item list, 

- what are the items prices,

- can the request be cancelled or not.

Then I will draw the state diagram. We will have 4 states:

1) Idle state, ready to get money

2) money inserted

3) item is selected

4) dispensing the item

Then I will write corresponding checks for the 2 and 3 states (to check if the money is acceptable, if the selected item is available and the money is enough, etc.)

16.You have two lightbulbs at a 100-story building. You want to find the floor at which the bulbs will break when dropped. How would you find the floor using the least number of drops?

The minimum number of tries is 14. First I will throw the 1st egg from the 14th store. If it is broken, I will throw the second egg starting from 1st store (if it is not broken in the 1st, then try from 2nd, etc.). In the worst case I will do 13 tries with the 2nd egg. (13+1= 14) If the 1st egg is not broken from the 14th store, then will throw it from 27th store (14+14-1). If it is broken, I will contrinue with the 2nd egg from the 26th store to 26th store sequentially. In worst case I will do 12 attempts. (12+2=14) So continueing this process, each time I will throw 1st egg from the store : 14, 14+14-1, 14+14+14-2, … and if it is broken, will throw the 2nd egg starting from the next store. To sum up, if we have N stores and need to find the minimal attempts number, we need to find the M number, for which the sum of 1 to M numbers is more or equal to N.

17.If you have a square room with no roof, and you had four pillars you had to plant on the walls so that each pillar touched two walls, how would you do it?

I would place the trees in the room corners. In this case each tree will touch 2 walls.If you have a square room with no roof, and you had four pillars you had to plant on the walls so that each pillar touched two walls, how would you do it?

18.Given 9 balls all of which weigh the same except for one, what is the minimum of weighings necessary to find the ball weighs more (or less)?

Let's divide the coins into 3 groups and name them A, B, C. The coins will be named A0, A1, A2, B0, B1, B2, C0, C1, C2.
The attempts will be the following:
 A with B.
    - If A is equal to B, 2nd attempt will be weigh C0 with C1, if equal, then the 3rd attempt will be C1 with C2. If C1 is more than C2, it means that C2 is that one coin, having less weigth, otherwise C2 have more weigth.
      If C0 is more or less than C1, then will compare C1 with C2. If C1=C2, then C0 is the different coin, and based on C0 was less then C1 or more, will decide if it has more wighth then others or less weigth.
    - If A is more than B, 2nd attempt will be B with C. If B is equal to C, it means that the differing coin is in the A group, and it has more weight than the others. Otherwise if B is less than C, then the differing coin is in B and it is with less wegth.
      Taking into acount that we know already the group of coins having different coin and also know the differing coin has lower or more weight, the 3rd attempt will be among 2 coins in the known group. If the coins are equal, then the 3rd one is that one, otherwise
      if one of the 2 has less weigth, than the based on info that we had (if the different coin had more or less wegth), the different coin will be found.
