Download Link: https://assignmentchef.com/product/solved-solved-determining-square-roots-using-newtons-method
<br>
Objective        To write a program that calculates square roots using Newton’s Method.

PROJECT DESCRIPTION

Write, compile and execute a complete program that prompts the user for a non  negative     real number, calls a method named Compute that uses Newton’s Method to compute            the square root of the number and then displays the square root to the user.  The   method prototype for method Compute and the driver program to test methodCompute is given in the program code in Figure 1, which follows.  Complete this code by adding the method definition of Compute.

A sample program output is given below.

Output

Program: find square roots by Newton’s Method

Please enter a number: 3

1.500001.7500010.25000

1.750001.7321420.01786

1.732141.7320530.00009

1.732051.7320540.00000

The square root of 3.00000 is 1.73205

Information about This Project

This particular program uses Newton’s Method, which is an example of an iterative process.  An iterative process is one which performs some task until a result is satisfied.

Newton’s Method for determining square roots is outlined in the steps which follow:

STEP 1             Prompt the user for R , the number whose square root is to be                                        determined.

STEP 2             Set x 0  =  R  ÷ 2

STEP 3             Compute an approximation of the square root of R  using the formula:

x n  +  1  =

x n

−

( x n  ) 2  −  R

2 x n

STEP 4             Repeat STEP 3 until | x n  +  1  −  x n  | is less than the desired level of                            accuracy.  When this level of accuracy has been reached, terminate the                           process and let x n  +  1 be a final approximation of the square root of R .

For the above example, x 0  =  3  ÷ 2  =  1.5

x 1  =  x 0  −  ( x 0 2  −  R  ) / ( 2 x 0 )

PROJECT     Determining Square Roots Using Newton’s Method

substitution yields

x 1  =  1.50  −  ( 1.50 2  −  3 ) / ( 2  ×  1.50 )  =  1.75

x 2  =  x 1  −  ( x 1 2  −  R  ) / ( 2 x 1 )

substitution yields

x 2  =  1.75  −  ( 1.75 2  −  3 ) / ( 2  ×  1.75 )  =  1.73214

x 3  =  x 2  −  ( x 2 2  −  R  ) / ( 2 x 2 )

substitution yields

x 3  =  1.73214  −  ( 1.73214 2  −  3 ) / ( 2  ×  1.73214 )  =  1.73205

x 4  =  x 3  −  ( x 3 2  −  R  ) / ( 2 x 3 )

substitution yields

x 4  =  1.73205  −  ( 1.73205 2  −  3 ) / ( 2  ×  1.73205 )  =  1.73205

Since x 4 and x 3 are approximately the same, the iterative process ceases and the square root of 3 is reported as 1.73205 .

Steps To Complete This Project

STEP 1             Open Eclipse and Write the Program Code

Open Eclipse, or JCreator or equivalent Java IDE on your computer.  Write the program code that will allow the user to enter the necessary input item(s) and then use these items to compute the required output value(s).

STEP 2             Compile and Run Your Program

Build, compile and run your program.  Test the operation of your program using                          appropriate numbers for your input variable(s).

STEP 3             Submit Your Program Code and Your Run Time Output

When completed, submit your program source code as well as the program                     output(s).

PROJECT     Determining Square Roots Using Newton’s Method

Figure 1           Method Definition and Driver Program for Newton Program

import java.text.DecimalFormat;

import java.util.Scanner;

public class Newton {

public static float Compute(float num)

{

float sqrRoot = 0;

// method definition

return sqrRoot;

}

public static void main(String[] args)

{

// declare a Scanner class object

Scanner sc = new Scanner(System.in);

// declare a DecimalFormat class object

DecimalFormat fourDecimal =  new DecimalFormat(“0.0000”);

float Number = 0;

System.out.println(“Program: find square roots byNewton’s Method”);

System.out.println(“Please enter a number: “);

Number = sc.nextFloat();

System.out.println(“The square root of ” + Number +” is ” + fourDecimal.format(Compute(Number)));

}

}