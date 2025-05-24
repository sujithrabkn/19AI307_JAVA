# Ex.No:6(D) PACKAGES

## AIM:
To create a Java Program for accessing package from another package using packagename.

## ALGORITHM :

1. Start the Program
2. Create a directory named pack and save A.java inside it.
3. Compile A.java from the parent directory using javac pack/A.java.
4. Create another directory named mypack and save B.java inside it.
5. Compile B.java from the parent directory using javac mypack/B.java.
6. Run B from the parent directory with java mypack.B

## PROGRAM:

```
Program to implement a Packages using Java
Developed by: SUJITHRA B K N
RegisterNumber: 212222230153
```

## Sourcecode.java:

```
package packageone;

public class Message {
    public void showMessage() {
        System.out.println("Hello from packageone!");
    }
}

package packagetwo;

import packageone.Message;  // Import the class from another package

public class PackageTest {
    public static void main(String[] args) {
        Message msg = new Message();  // Create object of class from another package
        msg.showMessage();
    }
}
```

## OUTPUT:

![442049563-cf76e54d-27ed-434b-824e-3ba7fb9421e1](https://github.com/user-attachments/assets/d6a84af2-2842-4a55-b21f-12fdb9f60ee8)

## RESULT:
Thus, the program has accessed the package from another package has been done successfully.
