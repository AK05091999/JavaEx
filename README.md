class Main {
  public static void main(String[] args) {

    int n = 10, firstTerm = 0, secondTerm = 1;
    System.out.println("Fibonacci Series till " + n + " terms:");

    for (int i = 1; i <= n; ++i) {
      System.out.print(firstTerm + ", ");

      // compute the next term
      int nextTerm = firstTerm + secondTerm;
      firstTerm = secondTerm;
      secondTerm = nextTerm;
    }
  }
}
Output

Fibonacci Series till 10 terms:
0, 1, 1, 2, 3, 5, 8, 13, 21, 34,
In the above program, firstTerm and secondTerm are initialized with 0 and 1 respectively (first two digits of Fibonacci series).

Here, we have used the for loop to

print the firstTerm of the series
compute nextTerm by adding firstTerm and secondTerm
assign value of secondTerm to firstTerm and nextTerm to secondTerm
We can also use a while loop to generate the Fibonacci series in Java.

Example 2: Display Fibonacci series using while loop
class Main {
  public static void main(String[] args) {

    int i = 1, n = 10, firstTerm = 0, secondTerm = 1;
    System.out.println("Fibonacci Series till " + n + " terms:");

    while (i <= n) {
      System.out.print(firstTerm + ", ");

      int nextTerm = firstTerm + secondTerm;
      firstTerm = secondTerm;
      secondTerm = nextTerm;

      i++;
    }
  }
}
Run Code
Output

Fibonacci Series till 10 terms:
0, 1, 1, 2, 3, 5, 8, 13, 21, 34,
The working of this program is the same as the previous program.

And, though both programs are technically correct, it is better to use a for loop in this case. It's because the number of iterations (from 1 to n) is known.

Example 3: Display Fibonacci series up to a given number
class Fibonacci {
  public static void main(String[] args) {

    int n = 100, firstTerm = 0, secondTerm = 1;
        
    System.out.println("Fibonacci Series Upto " + n + ": ");
    
    while (firstTerm <= n) {
      System.out.print(firstTerm + ", ");

      int nextTerm = firstTerm + secondTerm;
      firstTerm = secondTerm;
      secondTerm = nextTerm;

    }
  }
}
Run Code
Output

Fibonacci Series Upto 100:
0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 
In this example, instead of displaying the Fibonacci series of a certain number, we are displaying the series up to the given number (100).

For this, we just need to compare the firstTerm with n. And, if firstTerm is less than n, it is printed in the series. Else, the series is completed.

Share on:
Did you find this article helpful?

Related Examples
Java Example

Display Alphabets (A to Z) using loop

Java Example

Find Factorial of a Number

Java Example

Calculate Standard Deviation

Java Example

Check Armstrong Number


Join our newsletter for the latest updates.
Enter Email Address
Join


Tutorials
Python 3 Tutorial
JavaScript Tutorial
SQL Tutorial
HTML Tutorial
R Tutorial
C Tutorial
C++ Tutorial
Java Tutorial
Rust Tutorial
Go Tutorial
Kotlin Tutorial
Swift Tutorial
C# Tutorial
DSA Tutorial
Examples
Python Examples
JavaScript Examples
C Examples
Java Examples
Kotlin Examples
C++ Examples
Company
About
Advertising
Privacy Policy
Terms & Conditions
Contact
Blog
Careers
Youtube
Apps
Learn Python
Learn C Programming
Learn Java
© Parewa Labs Pvt. Ltd. All rights reserved.

   
