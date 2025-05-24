# Ex.No:4(D) FINAL & STATIC IN JAVA

## AIM:
To create a Java program for below situation, Student object contains member 'Stu_Id'. It contains object named subject, which contains its own informations such as subject1,subject2,subject3,subject4.

## ALGORITHM :

1. Start
2. Define class Subject:

   Declare four String variables: subject1, subject2, subject3, subject4.

3. Define method dispSub(String s1, String s2, String s3, String s4):

   Assign s1 to subject1.

   Assign s2 to subject2.

   Assign s3 to subject3.

   Assign s4 to subject4.

   Print the four subject names together with spaces between them.

4. Define class Student:

   Declare an int variable Stu_Id.

   Create an object sub of the Subject class.

5. Define method disp(int id, String s1, String s2, String s3, String s4):

   Assign id to Stu_Id.

   Print Stu_Id.

   Call dispSub method of sub object, passing the four subject names s1, s2, s3, and s4.

6. Define class Main:

   In the main method:

   Create an object st of Student class.

7. Call the disp method on st, passing:

   Student ID: 101

   Subjects: "Java", "DS", "TOC", "CG"

8. End

## PROGRAM:

```
Program to implement a final & Static using Java
Developed by: SUJITHRA B K N
RegisterNumber: 212222230153
```

## Sourcecode.java:

```
class Subject {
    String subject1, subject2, subject3, subject4;

    void dispSub(String s1, String s2, String s3, String s4) {
        subject1 = s1;
        subject2 = s2;
        subject3 = s3;
        subject4 = s4;
        System.out.println(subject1 + " " + subject2 + " " + subject3 + " " + subject4);
    }
}

class Student {
    int Stu_Id;
    Subject sub = new Subject();

    void disp(int id, String s1, String s2, String s3, String s4) {
        Stu_Id = id;
        System.out.println(Stu_Id);
        sub.dispSub(s1, s2, s3, s4);
    }
}

public class Main {
    public static void main(String[] args) {
        Student st = new Student();
        st.disp(101, "Java", "DS", "TOC", "CG");
    }
}
```

## OUTPUT:

![438025781-70c0a76a-f3e3-49f4-9590-84e1f38706ef](https://github.com/user-attachments/assets/7586448a-8927-4199-af97-1be446eb9ddd)

## RESULT:
Thus, the java program for below situation, Student object contains member 'Stu_Id'. It contains object named subject, which contains its own informations such as subject1,subject2,subject3,subject was executed successfully.
