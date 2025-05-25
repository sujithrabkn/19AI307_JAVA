# Ex.No:9(D) TRANSIENT ---SERILIZATION

## AIM:
To implement a Java program to perform Transient in Employee details in Serializable interface to make its object serialized.

## ALGORITHM :

1. Get employee name and designation from the user.
2. Save the Employeeinfo object to emp.txt.
3. Read the object back from emp.txt.
4. Print employee name and designation (designation is null due to transient).
5. Delete File: Delete emp.txt and handle any exceptions while trying to read it.

## PROGRAM:
```
/*
Program to implement a Transient using Java
Developed by: SUJITHRA B K N
RegisterNumber: 212222230153
*/
```

## Sourcecode.java:

```
class Employeeinfo implements Serializable
{
    String name;
    String desi;
    transient int id;
   
    Employeeinfo(String n, String r, int na)
    {
    this.name = n;
    this.desi = r;
    this.id=na;
   
    }
}
```

## OUTPUT:

![440202764-faf0d5f6-9998-4d44-b586-b3c706536431](https://github.com/user-attachments/assets/7a790046-f357-4d76-a179-71828947043c)

## RESULT:
Thus, implementation of a Java program to perform Transient in Employee details in Serializable interface to make its object serialized was executed and verified successfully.
