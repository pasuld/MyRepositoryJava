import java.util.Scanner;

public class Ex.Class.05.08.25 {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter an integer value:");

        int n = sc.nextInt();

        // If x is even, x = x / 2
        // If x is odd, x = 3 * x + 1
        /*
         * The program will stop when x reaches the final value of 1.
         * For example, for x = 13, the output will be:
         * 40 -> 20 -> 10 -> 5 -> 16 -> 8 -> 4 -> 2 -> 1
         */

        System.out.print(n); // To include the starting value
        while (n != 1) {
            if (n % 2 != 0) {
                n = n * 3 + 1;
            } else {
                n = n / 2;
            }
            System.out.print(" -> " + n);
        }
    }
}
