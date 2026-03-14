# java-test-0004-final-15325-sushant
Final Project Assignment - This repository contains the complete final project code and documentation.
public class Main {
    public static void main(String[] args) {
        int n = 4;
        int size = 2 * n - 1;
        int center = n - 1;

        for (int i = 0; i < size; i++) {
            for (int j = 0; j < size; j++) {
                int rowDistance = Math.abs(i - center);
                int colDistance = Math.abs(j - center);

                int value = Math.max(rowDistance, colDistance) + 1;

                System.out.print(value);
                if (j < size - 1) {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }
    }
}
