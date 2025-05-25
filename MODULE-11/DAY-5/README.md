# Ex.No:11(E) JAVA HASHMAP

## AIM:
To Write a Java program to get the first and last elements in a tree set.

## ALGORITHM :

a.	Import java.util.*.

b.	Start the program and create a Scanner to take input from the user.

c.	Read an integer size, then loop to take size number of string inputs and insert them into the TreeSet.

d.	Print the entire TreeSet, which displays the elements in sorted order.

## PROGRAM:
```
/*
Program to implement a HASHMAP
Developed by: SUJITHRA B K N
RegisterNumber: 212222230153
*/
```

## Sourcecode.java:

```
import java.util.*;
public class Exercise5 {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int size=sc.nextInt();
        TreeSet<String> tree_set = new TreeSet<String>();
        for(int i=0;i<size;i++){
            tree_set.add(sc.next());
        }
        System.out.println("Tree set: ");
        System.out.println(tree_set);
        Object first_element = tree_set.first();
        System.out.println("First Element is: "+first_element);
        Object last_element = tree_set.last();
        System.out.println("Last Element is: "+last_element);
        
    }
}
```

## OUTPUT:

![443968744-c1960a72-3798-40be-8801-1b2e16180c24](https://github.com/user-attachments/assets/64be10d2-5b5f-4bee-a038-837e9493252d)


## RESULT:
Thus the java program was successfully executed.
