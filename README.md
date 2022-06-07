# powerRecursive
import java.util.Scanner;

public class Main {

    static int power(int taban, int us) {
        int result = 1;
        if (us == 0) {
            return 1;
        }
        for (int i = 1; i <= us; i++) {
            result = taban * power(taban, us - 1);
        }
        return result;
    }

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.println("tabani giriniz : ");
        int taban = input.nextInt();
        System.out.println("us giriniz : ");
        int us = input.nextInt();

        System.out.println("us : " + power(taban, us));


    }
}
