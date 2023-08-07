INPT is receiving new students for the year 2023/2024.
Student are given a paper holding a number from 1 to 10, and each student enter the institut in turn after he passes his paper to the student behind him, each student is requested to answer this question before entering: what is the total of the numbers written in the papers you are currently possessing?

Example: 
- array[1,2,3,4,5,6,7,8,9]
- answer: [1,3,6,10,15,21,28,36,45,55]

code:
```java
import java.util.ArrayList;
import java.util.Scanner;

public class test {

    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        
        int t = s.nextInt();
        
        ArrayList<Integer> test = new ArrayList<Integer>(t);
        
        for (int i = 0; i < t; i++) {
            int r = s.nextInt();
            test.add(r);
        }
        
        ArrayList<Integer> ans = new ArrayList<Integer>(t);
        
       
        int saver = 0;
        
        for (int j = 0; j < test.size(); j++) {
            saver += test.get(j);
            ans.add(saver);
        }
        
        System.out.println(ans);
        
        s.close();
    }
}
```