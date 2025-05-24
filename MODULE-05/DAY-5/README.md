# Ex.No:5(E) HAS-A RELATIONSHIP

## AIM:
To implement a java program for area of triangle with the help of getter and setter method and to print the value of area of triangle.

## ALGORITHM :

1. Start the program and import Scanner for user input.
2. Create a TriangleArea class with:

   Private variables width and height.

   Methods setWidth(double) and setHeight(double) to assign values.

   Method getArea() that returns the area by multiplying width and height.

3. In the main method:

   Create a Scanner object and a TriangleArea object.

   Read two double inputs from the user (for width and height).

   Set the width and height in the TriangleArea object and calculate the area.

   Print the area (after converting it to an integer) and close the scanner.

## PROGRAM:

```
Program to implement a HAS-A RelationShip
Developed by: SUJITHRA B K N
RegisterNumber: 212222230153
```

## Sourcecode.java:

```
import java.util.Scanner;
public class TriangleArea {

    private double width;
    private double height;

    public void setWidth(double width) {
        this.width = width;
    }

    public void setHeight(double height) {
        this.height = height;
    }

    public double getArea() {
        return width * height;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        TriangleArea triangle = new TriangleArea();
        double w = sc.nextDouble(); 
        double h = sc.nextDouble(); 
        triangle.setWidth(w);
        triangle.setHeight(h);
        System.out.println((int)triangle.getArea());
    }
}
```

## OUTPUT:

![438033209-6761079b-9734-42e3-bbcd-705e07963810](https://github.com/user-attachments/assets/0ce4b075-228c-488f-92e4-5046f5c656d9)


## RESULT:
Thus the java program to Find the Largest or Max Number in Array using has - a relationship was executed successfully.
