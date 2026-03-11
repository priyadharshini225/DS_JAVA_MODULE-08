# Ex11 Convert HashSet to ArrayList in Java
## DATE: 11/03/26
## AIM:
To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
## Algorithm
1. Start the program.
2. Read n
3. Insert elements into a HashSet.
4. Create an ArrayList from the HashSet.
5. Print ArrayList elements.   

## Program:
```
/*
Program to To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
Developed by: PRIYADHARSHINI S
RegisterNumber: 212223240129 
*/

import java.util.*;

public class HashSetToArrayList {

    public static ArrayList<Integer> convertToArrayList(HashSet<Integer> set) {
        return new ArrayList<>(set);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        HashSet<Integer> set = new HashSet<>();
        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            set.add(num);
        }

        ArrayList<Integer> list = convertToArrayList(set);
        System.out.println("ArrayList contents:");
        for (int num : list) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}
```

## Output:

<img width="661" height="714" alt="image" src="https://github.com/user-attachments/assets/3e9d21b2-47e8-4f18-9551-a868d5321305" />


## Result:
The program successfully converts a collection of distinct integers stored in a HashSet into an ArrayList
