# Ex.No:5(C) GETTER AND SETTER METHOD

## AIM:
To Create a java program to print fibonacci series for given number , to read and display the value with the help of setter and getter method.

## ALGORITHM :

1. Start the program and import Scanner to take user input.
2. Create a Fibonacci class with:

   A private int variable count.

   Methods setCount(int) to set the number of terms and getCount() to retrieve it.

   A printSeries() method to generate and print the Fibonacci series using a loop.

3. In the Main class:

   Create a Scanner object and a Fibonacci object.

   Read an integer input from the user to decide how many terms to generate.

   Set the count in the Fibonacci object and call printSeries() to display the series.

4. Close the Scanner and end the program.

## PROGRAM:


```
Program to implement a Getter and Setter using Java
Developed by: SUJITHRA B K N
RegisterNumber: 212222230153
```

## Sourcecode.java:

```
import java.util.Scanner;

class Fibonacci {
    private int count;

    public void setCount(int count) {
        this.count = count;
    }

    public int getCount() {
        return count;
    }

    public void printSeries() {
        int n1 = 0, n2 = 1;
        for (int i = 0; i < count; i++) {
            System.out.print(n1 + " ");
            int next = n1 + n2;
            n1 = n2;
            n2 = next;
        }
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Fibonacci fib = new Fibonacci();

        int input = sc.nextInt();
        fib.setCount(input);
        fib.printSeries();

        sc.close();
    }
}
```

## OUTPUT:

![438031518-3f2c59a9-3be2-4162-af36-f7a26eb2f318](https://github.com/user-attachments/assets/c22d9eb1-5326-4a57-b6e2-c73455e623b6)

## RESULT:
Thus the java program to print fibonacci series for given number , to read and display the value with the help of setter and getter method.was executed successfully.
