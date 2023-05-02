Download Link: https://assignmentchef.com/product/solved-comp2120-assignment-3
<br>
Credit Card Number Validation: In this problem, your job is to validate a credit card number given by the user as a String. First, remove all the spaces or dashes between the number. (Remember that the number is given as a string.) Then, do the following steps to validate the number:

<ul>

 <li>Form the sum of all the digits of the credit card number.</li>

 <li>Add to that sum every second digit, starting with the second digit from the right.</li>

 <li>Add the number of digits in the second step that are greater than 4.</li>

 <li>The result should be divisible by 10.</li>

</ul>

For example, consider the number 4012 8888 8888 1881. The sum of all digits is 89. The sum of the colored digits is 46. There are five colored digits larger than 4, so the result is 89+46+5=140. This final number, 140, is divisible by 10, so the card number is valid.

Write a Java program, to create a class for this problem, including a method to check the validity of a given number. Then, write a tester program to test some 16-digits numbers for their validity to be credit card numbers.







Problem 2.       (25 points)

Complete the two Java programs below. The first one, PrimeGenerator, generates prime numbers, and the second one, prompts the user for an integer, and then prints out all prime numbers up to that integer. For example, when the user enters 10, the program should print:

2

3

5

7




<em>/** </em>

<em>   This class generates all prime numbers. </em>

<em>*/ </em>

<strong>public class </strong>PrimeGenerator

{

<strong>private int </strong><strong>current</strong>;




<strong>public </strong>PrimeGenerator()

{

<strong>current </strong>= 1;

}

<em>/** </em>

<em>      Calculates the next prime number. </em>

<em>      <strong>@return </strong>the next prime number </em>

<em>   */ </em>

<em>   </em><strong>public int </strong>nextPrime()

{

<strong>     // Complete this part </strong>

<strong>     …</strong>

}




<em>/** </em>

<em>      Check if n is a prime number. </em>

<em>      @param n to check whether it is prime or not </em>

<em>      <strong>@return </strong>true if n is prime </em>

<em>   */ </em>

<strong>public static boolean </strong>isPrime(<strong>int </strong>n)

{

<strong>     // Complete this part </strong>

<strong>     …</strong>

}

}




<strong>import </strong>java.util.Scanner;




<em>/** </em>

<em>   This class prints prime numbers. </em>

<em>*/ </em>

<strong>public class </strong>PrimePrinter

{

<strong>public static void </strong>main (String[] args)

{

Scanner in = <strong>new </strong>Scanner(System.<strong><em>in</em></strong>);       System.<strong><em>out</em></strong>.print(<strong>“Enter upper limit: “</strong>);       <strong>int </strong>limit = in.nextInt();




<strong>      // Complete this part </strong><strong>      … </strong>




} }







Problem 3.       (25 points)

Tic-Tac-Toe: Write a Java program that plays tic-tac-toe. The tic-tac-toe game is played on a 3X3 grid. The game is played by two players, who take turns. The first player marks a cell with a circle, the second one another cell with a cross. The player who has formed a horizontal, vertical, or diagonal sequence of three marks wins. Your program should draw the game board, ask the user for the coordinates of the next mark, redraw the board, change the players after every successful move, and announce the winner.




<strong>Note</strong>: You don’t need to create a graphical user interface for this program. You can just draw the board using some characters on the terminal like below:




|      |  o

———–

|  x  |

———–     |  o  |  x







Problem 4.       (25 points)

You are given a two-dimensional array of values that specify the height of a terrain at different points in a square. Write a Java program with the following tasks:

<ul>

 <li>A method to read the heights of all the points of a terrain and store them into the two-dimensional array. You can assume that the heights are integer values.</li>

 <li>Constructor of the class</li>

 <li>A method to find the lowest point of the terrain.</li>

 <li>A method to find the highest point of the terrain.</li>

 <li>A method to print out a flood map, showing which of the points in the terrain would be flooded if the water level was a given value. In the flood map, print a * for each flooded point and a – for each point that is not flooded. Here is a sample map for a 5 by 5 square:</li>

</ul>




<ul>

 <li>* – * –</li>

 <li>– – * *</li>

 <li>* * * *</li>

</ul>

– – * – *

<ul>

 <li>* – – –</li>

</ul>

Test your implemented class using a 4 by 4 squared terrain.




<strong>Note</strong>: Your main class should work for squared terrains with