# Ex.No:5(A) DATA HIDING AND ENCAPSULATION

## AIM:
To Create a java program to display the age of the person.Use access modifier private to achieve the data hiding concepts.

## ALGORITHM :

1. Start
2. Import the Scanner class for input.
3. Define class Person:

   Declare a private int variable age.

4. Create a method setAge(int age):
5. Assign the input parameter age to the instance variable age.
6. Create a method getAge():

   Return the value of age.

7. Define class Main:
8. In the main method:

   Create a Scanner object scanner to read user input.

   Create an object p of class Person.

   Read an integer from the user and store it in inputAge.

   Call p.setAge(inputAge) to set the age in the Person object.

   Print "My age is " followed by the value returned by p.getAge().

   Close the scanner.

9. End

## PROGRAM:

```
Program to implement a Data Hiding & Encapsulation using Java
Developed by: SUJITHRA B K N
RegisterNumber: 212222230153
```

## Sourcecode.java:

```
import java.util.Scanner;

class Person {
    private int age;

    public void setAge(int age) {
        this.age = age;
    }

    public int getAge() {
        return age;
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        Person p = new Person();

        int inputAge = scanner.nextInt();
        p.setAge(inputAge);

        System.out.println("My age is " + p.getAge());
        scanner.close();
    }
}
```

## OUTPUT:

![438029194-781fdc29-385a-4a25-bdb3-72d4c304f256](https://github.com/user-attachments/assets/f82319b9-dd88-402c-b318-924b1df305d3)

## RESULT:
Thus , the java program to display the age of the person.Use access modifier private to achieve the data hiding concepts.
