import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.util.Arrays;

public class BinarySearch {

    public static void main(String[] args) {
        BufferedReader input = new BufferedReader(new InputStreamReader(System.in));
        try {
            System.out.print("Masukkan angka : ");
            int index = 0;
            int number = Integer.parseInt(input.readLine());
            int[] binary = { 11, 2, 7, 1, 3, 32, 39, 66, 46, 28, 90, 88 };
            int binaryLen = binary.length; // len(array)
            for (int x : binary) { // for x in array
                if (number == x) {
                    System.out.println("Angka ditemukan pada index ke-" + index);
                    break;
                }
                index++;
            }
            if (index == binaryLen) {
                System.out.println("Angka tidak ditemukan");
            }
        } catch (IOException exception) {
            System.out.println("Input Error!");
        }
    }
    
}