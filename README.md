import java.util.Scanner;

public class TestArray {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        double[] myList = new double[10];

        System.out.print("Enter " + myList.length + " values: ");
        for (int i = 0; i < myList.length; i++) {
            myList[i] = input.nextDouble();
        }

        System.out.println("\nGenerated Custom Random Numbers:");
        System.out.println("Integer (0–100): " + CustomRandom.getRandom(100));
        System.out.println("Integer (10–50): " + CustomRandom.getRandom(10, 50));
        System.out.println("Double (0–1): " + CustomRandom.getRandom());
        System.out.println("Double (0–10): " + CustomRandom.getRandom(10.0));
        System.out.println("Float (0–5): " + CustomRandom.getRandom(5.0f));

        input.close();
    }
}
