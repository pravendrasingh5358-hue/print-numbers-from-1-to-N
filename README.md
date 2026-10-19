# print-numbers-from-1-to-N
import java.util.Scanner;

public class Solution {
    
    // Recursive method to print numbers from 1 to N
    public static void printNumbers(int n) {
        // Base case: stop when N reaches 0
        if (n == 0) {
            return;
        }
        
        // Recursive call for (N - 1)
        printNumbers(n - 1);
        
        // Print the current number after returning from recursive calls
        System.out.print(n + " ");
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        if (sc.hasNextInt()) {
            int n = sc.nextInt();
            printNumbers(n);
        }
        sc.close();
    }
}
