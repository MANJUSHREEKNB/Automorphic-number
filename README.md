# Automorphic-number
AUTOMORPHIC NUMBER
Follow the steps given below:
1.	Read a number (num) from the user.
2.	Find the square of the given number and store it in a variable (square).
3.	Find the last digit(s) of the square.
4.	Compare the last digit(s) of the variable with num.
5.	If they are not equal, the given number is not an automorphic number.
6.	If they are the same, go to the next step.
7.	Remove the last digit of the given number i.e. num.
8.	Repeat steps 4 to 6 until the given number becomes 0.
Java Automorphic Number Program
import java.io.*;
import java.util.*;
public class AutomorphicNumberExample1  
{   
static boolean isAutomorphic(int num)   
{   
int square = num * num;   
while (num > 0)   
{   
if (num % 10 != square % 10)   
return false;   
num = num/10;   
square = square/10;   
}   
return true;   
}   
public static void main(String args[])   
{   
System.out.println(isAutomorphic(76) ? "Automorphic" : "Not Automorphic");   
System.out.println(isAutomorphic(13) ? "Automorphic" : "Not Automorphic");   
}   
}  
OUTPUT :
Automorphic
Not Automorphic

