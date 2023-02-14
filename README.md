# Java Journey, 05: Loops

In programming, loops are used to execute a block of code repeatedly until a certain condition is met. They provide a way to iterate through a sequence of values, such as the elements of an array or the characters in a string. There are several types of loops available in Java, including for loops, while loops, and do-while loops, each with their own unique features and use cases.

## For Loop

A for loop in Java is a control structure that is used to repeat a block of code a certain number of times. The general syntax of a for loop is:

```bash
for (initialization; condition; increment/decrement) {
    // code to be repeated
}
```

The "initialization" statement is executed only once before the loop starts, and it usually initializes a counter variable. The "condition" is checked at the beginning of each loop iteration, and if it is true, the block of code inside the loop is executed. The "increment/decrement" statement is executed at the end of each loop iteration and it usually updates the counter variable.

For example, the following for loop prints the numbers from 1 to 10:

```bash
for (int i = 1; i <= 10; i++) {
    System.out.println(i);
}
```

In this loop, the variable "i" is initialized to 1, the condition "i <= 10" is checked before each iteration, and the increment "i++" is executed at the end of each iteration. The loop will execute 10 times, and each time it will print the value of "i".

The for loop is often used when the number of iterations is known beforehand, and it can be more concise and readable than a while loop in these cases. It can also be used to iterate over arrays or other collections.

## While Loop

In Java, a "while" loop is used to execute a set of statements repeatedly until a specific condition is met. It is a pre-test loop, which means that the condition is checked before executing the statements inside the loop.

The basic syntax of a "while" loop is as follows:

```bash
while (condition) {
    // statements to be executed
}
```

The condition in a "while" loop can be any Boolean expression that evaluates to "true" or "false". If the condition is "true", the statements inside the loop are executed. If the condition is "false", the loop is exited and the program continues with the next statement after the loop.

Here is an example of a simple "while" loop that prints the numbers from 1 to 10:

```bash
int i = 1;

while (i <= 10) {
    System.out.println(i);
    i++;
}
```

n this example, the loop will continue to execute as long as the value of i is less than or equal to 10. The println() statement inside the loop will print the value of i to the console, and the value of i will be incremented by 1 at the end of each iteration of the loop.

While loops can be useful when you don't know in advance how many times you need to execute a set of statements, or when you need to repeat a set of statements until a specific condition is met.

## Do-While Loop

The do-while loop in Java is a control flow statement that allows code to be executed repeatedly based on a given condition. It is similar to the while loop, with the main difference being that the do-while loop guarantees that the loop body is executed at least once, regardless of whether the condition is true or false.

The syntax of the do-while loop is as follows:

```bash
do {
   // loop body
} while (condition);
```

The loop body is executed first, and then the condition is evaluated. If the condition is true, the loop body is executed again. This continues until the condition becomes false, at which point control is transferred to the next statement after the loop.

Here is an example of a do-while loop that asks the user to input a number until a valid number is entered:

```bash
import java.util.Scanner;

public class DoWhileExample {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      int number;

      do {
         System.out.print("Enter a number between 1 and 10: ");
         number = input.nextInt();
      } while (number < 1 || number > 10);

      System.out.println("You entered: " + number);
   }
}
```

In this example, the loop body asks the user to input a number. If the number is less than 1 or greater than 10, the loop continues and the user is asked to input another number. If a valid number is entered, the loop terminates and the program prints the number.
