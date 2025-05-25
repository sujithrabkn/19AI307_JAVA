# Ex.No:12(B) COMPARABLE & COMPARATOR INTERFACE

## AIM :
To Write a java program to sort the list based on null value for name using comparator method(nullsfirst).

## ALGORITHM :

1. Define Student class with rollno, name, and age attributes.
2. Create constructor and getter/setter methods.
3. Instantiate an ArrayList.
4. Add Student objects to the list (including one with null name).
5. Define a Comparator using Comparator.comparing() with Comparator.nullsFirst().
6. Sort the list using Collections.sort() with the defined comparator.
7. Iterate through the sorted list and print student details.

## PROGRAM:
```
/*
Program to implement a COMPARABLE & COMPARATOR INTERFACE using Java
Developed by: SUJITHRA B K N
RegisterNumber: 212222230153
*/
```

## Sourcecode.java:

```
import java.util.*;    
 class Student {    
   int rollno;    
   String name;    
  int age;    
    Student(int rollno,String name,int age){    
    this.rollno=rollno;    
    this.name=name;    
    this.age=age;    
    }  
    public int getRollno() {  
        return rollno;  
    }  
    public void setRollno(int rollno) {  
        this.rollno = rollno;  
    }  
    public String getName() {  
        return name;  
    }  
  
    public void setName(String name) {  
        this.name = name;  
    }  
  
    public int getAge() {  
        return age;  
    }  
    public void setAge(int age) {  
        this.age = age;  
    }  
    }    public class TestSort2{    
 public static void main(String args[]){    
 ArrayList<Student> al=new ArrayList<Student>();    
 al.add(new Student(101,"Vijay",23));    
 al.add(new Student(106,"Ajay",27));    
 al.add(new Student(105,null,21));    
 Comparator<Student> cm1=Comparator.comparing(Student::getName,Comparator.nullsFirst(String::compareTo));  
  Collections.sort(al,cm1);  
  System.out.println("Considers null to be less than non-null");  
  for(Student st: al){  
     System.out.println(st.rollno+" "+st.name+" "+st.age);  
     }  
  
 }    
 }
```
   
## OUTPUT:

![444604054-6b268751-878d-4fc3-acec-edeb1682f905](https://github.com/user-attachments/assets/09e355a8-1f5b-4734-81ba-b98d39e69f35)

## RESULT:
Thus the java program to compare two elements , if element is greater means display 1 otherwise display -1 use only comparable interface in java collection was executed successfully.
