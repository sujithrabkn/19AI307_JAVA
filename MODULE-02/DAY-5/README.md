# Ex.No:2(E) SMALLEST ELEMENT IN AN ARRAY

## AIM:
To Write a Java program to find the largest element in an array and then print the largest value.

## ALGORITHM :
1.Start

2.Input the size of the array (let's call it size)

3.Create an integer array of length size

4.Loop from i = 0 to size - 1:,Input the i-th element and store it in the array

5.Initialize a variable largest with the first element of the array

6.Loop from i = 1 to size - 1:,If the current element array[i] is greater than largest:,Update largest = array[i]

7.Output the value of largest as the largest element

8.End

## PROGRAM:
```
/*
Program to implement a Smallest Element in an Array
Developed by: SUJITHRA B K N
RegisterNumber: 212222230153
*/
```

## Sourcecode.java:

```
import java.util.Scanner;
public class LargestElement {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int size = scanner.nextInt();
        int[] array = new int[size];
        for (int i = 0; i < size; i++) {
            array[i] = scanner.nextInt();
        }
        int largest = array[0]; // Assume the first element is the largest initially
        for (int i = 1; i < size; i++) {
            if (array[i] > largest) {
                largest = array[i];
            }
        }
        System.out.println("The largest element in the array is: " + largest);
        scanner.close();
    }
}
```

## OUTPUT:

![437409706-87908cbe-caef-4359-951a-178115c6dbdc](https://github.com/user-attachments/assets/8174072f-c34b-47cc-89c7-5c19b8fb80c0)

## RESULT:
Thus the java program successfully reads the array size and elements from the user and correctly finds and prints the smallest number in the array.
