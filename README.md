# differScannersPrinting
printing Scanners in different ways using next(); nextLine(); nextInt(); nextDouble(); nextBigDecimal(); nextBigInteger();

package scanners;

import java.math.BigDecimal;
import java.math.BigInteger;
import java.util.Scanner;

public class javaScannerNextLine {
	public static void main(String[] args) {
		
		Scanner input = new Scanner (System.in);
		
		System.out.print("\rEnter first name: ");
		String fname = input.nextLine();
		System.out.println("Using nextLine(): " + fname + "\n");
		
		System.out.print("Enter greeting: ");
		String value = input.next();
		System.out.print("Using next(): "+ value + "\n");
		//printing nextBigInteger() repeatedly...
		System.out.print("\rEnter big int num: ");
		BigInteger bigInt = input.nextBigInteger();
		System.out.println("Using nextBigInteger(): " + bigInt + "\n");
		
		System.out.print("\rEnter big int num again: ");
		BigInteger secondbigInt = input.nextBigInteger();
		System.out.println("Using nextBigInteger(): " + secondbigInt + "\n");
		
		System.out.print("\rEnter big decimal: "); //input
		BigDecimal bigDec = input.nextBigDecimal(); //stored
		System.out.println("Using nextBigDecimal(): " + bigDec + "\n"); //print
		
		System.out.print("\rEnter double number: ");
		Double doub = input.nextDouble();
		System.out.println("Using nextDouble: " + doub + "\n");
		
		System.out.print("\rEnter integer number: ");
		int intnum = input.nextInt();
		System.out.println("Using nextInt() : " + intnum + "\n");
		
		
		
		//used new scanner to print the String using nextLine(); in which is repeating
		Scanner newScanner1 = new Scanner(System.in);
		
		System.out.print("\rEnter place: ");
		String testplace = newScanner1.nextLine(); 
		System.out.println("Using nextLine(): " + testplace + "\n");
		
		//print everything
		System.out.println("Using next(): " + value + "\r " +
						   	"Using nextLine(): " + fname + "\r " +
							"Using nextBigInteger(): " + bigInt + "\r " +
						   	"Using nextBigInteger(): " + secondbigInt + "\r " +
							"Using nextBigDecimal(): " + bigDec + "\r " +
							"Using nextLine(); again in new Scanner: " +testplace + "\r " +
							"Using nextDouble() : " + doub + "\r " + 
							"Using nextInt() : " + intnum);
		
		input.close();
	}
}
/*using nextLine(); prints multiple lines of words while next(); only prints a single line of word */
