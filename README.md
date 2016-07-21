# CheckPowerOfTwo
import java.util.Scanner;

public class PowOfTwo {

	public static void main(String[] args) {
		Scanner qq = new Scanner(System.in);
		System.out.println("Enter a number :");
		int given = qq.nextInt();
		int ind = 0;
		int sub = 0;
		while (given > 2) {
			sub = given % 2;
			if (sub == 1) {
				ind = 1;
				break;
			} else {
				given = given / 2;
			}
		}
		if (ind == 1) {
			System.out.println("it is not a power of 2");
		} else {
			System.out.println("It is  a power of 2");
		}

	}

}
