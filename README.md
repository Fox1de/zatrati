import java.util.Random;
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Введите кол-во дней: ");
        int lenght = scanner.nextInt();
        int[] days = new int[lenght];
        Random random = new Random();
        for (int i = 0; i < lenght; i++) {
            days[i] = random.nextInt(10);
            System.out.println("В день, было потрачено: " + days[i]);
        }
        int sum = 0;
        for (int i = 0; i < lenght; i++) {
            sum = sum + days[i];
        }
        System.out.println("Суммарно было потрачено: " + sum);
    }
}
