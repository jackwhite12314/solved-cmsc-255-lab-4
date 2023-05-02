Download Link: https://assignmentchef.com/product/solved-cmsc-255-lab-4
<br>
Big Java, Late Objects / Java for Everyone, 2e

Chapter Number: 3 Decisions




1) Copy and run the following program. Explain how the program compares the two strings. How can you modify the program so that str2 and str3 are equal when they are compared?




public class StringEqual{   public static void main(String[] args)   {      String str1 = “abcd”;      String str2 = “abcdefg”;      String str3 = str1 + “efg”;      System.out.println(“str2 = ” + str2);      System.out.println(“str3 = ” + str3);      if (str2 == str3)      {         System.out.println(“The strings are equal”);      }      else      {         System.out.println(“The strings are not equal”);      }   }}










2) Remember the childhood game “Rock, Paper, Scissors”? It is a two-player game in which each person simultaneously chooses either rock, paper, or scissors. Rock beats scissors but loses to paper, paper beats rock but loses to scissors, and scissors beats paper but loses to rock. The following code prompts player 1 and player 2 to each enter a string: rock, paper, or scissors. Finish the code by adding nested if statements to appropriately report “Player 1 wins”, “Player 2 wins”, or “It is a tie.”




import java.util.Scanner;public class RockPaperScissors{     public static void main(String[] args)    {        Scanner scan = new Scanner(System.in);        System.out.println(“Player 1: Choose rock, scissors, or paper:”);        String player1 = scan.next().toLowerCase();        System.out.println(“Player 2: Choose rock, scissors, or paper:”);        String player2 = scan.next().toLowerCase();         (your code goes here…)    }}







3) The program in Lab 3.7 was heavily nested with if statements, and it can be difficult to follow the logic of any program that is heavily nested in this way. By constructing complex conditions with the &amp;&amp; operator, it is possible to simplify the code and remove some of the else alternatives. Rewrite the program in Lab 3.7 using complex conditions and omitting the else construct.







4) Draw a flowchart for a program that reads two integers and prints the smaller number.













5.1) Write a program that prompts the user to enter three strings. Compare the String objects lexicographically and print the middle-valued string. For example, if the three strings were “abcd”, “wxyz”, and “pqrs”, the program would print “pqrs”. Limit yourself to simple, nested if statements that don’t use the Boolean operators &amp;&amp; or ||. Be sure and test your code by giving it input data that tests every path through your code. Make a list of values for str1, str2, and str3 that would thoroughly test the code.







5.2) Rewrite the program solution for Lab 3.10.1 using the Boolean operator &amp;&amp; to simplify the logical structure.







6.1) Build and run the following program. What happens when the two points have the same <em>x</em>-coordinate?




import java.util.Scanner; public class Slope {   public static void main(String[] args)   {      Scanner in = new Scanner(System.in);       System.out.print(“Input x coordinate of the first point: “);      double xcoord1 = in.nextDouble();       System.out.print(“Input y coordinate of the first point: “);      double ycoord1 = in.nextDouble();       System.out.print(“Input x coordinate of the second point: “);      double xcoord2 = in.nextDouble();       System.out.print(“Input y coordinate of the second point: “);      double ycoord2 = in.nextDouble();       double slope = (ycoord2 – ycoord1) / (xcoord2 – xcoord1);              System.out.println(“The slope of the line is ” + slope);   } }







6.2) Correct and rebuild the slope program to disallow a vertical line (denominator = 0).








