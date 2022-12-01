# differScannersPrinting
printing Scanners in different ways using next(); nextLine(); nextInt(); nextDouble(); nextBigDecimal(); nextBigInteger();

package scanners;

import java.math.BigDecimal;
import java.math.BigInteger;
import java.util.Scanner;

public class javaScannerNextLine {
	public static void main(String[] args) {
		
		Scanner input = new Scanner (System.in);
		
		System.out.print("Enter greeting: ");
		String value = input.nextLine();
		System.out.print("Using nextLine(): "+ value + "\n");
		//printing nextBigInteger() repeatedly...
		System.out.println("\rEnter big int num: ");
		BigInteger bigInt = input.nextBigInteger();
		System.out.println("Using nextBigInteger(): " + bigInt + "\n");
		
		System.out.println("\rEnter big int num: ");
		BigInteger secondbigInt = input.nextBigInteger();
		System.out.println("Using nextBigInteger(): " + secondbigInt + "\n");
		
		System.out.println("\rEnter big decimal: "); //input
		BigDecimal bigDec = input.nextBigDecimal(); //stored
		System.out.println("Using nextBigDecimal(): " + bigDec + "\n"); //print
		
		System.out.println("\rEnter double number: ");
		Double doub = input.nextDouble();
		System.out.println("Using next(): " + doub + "\n");
		
		System.out.println("\rEnter integer number: ");
		int intnum = input.nextInt();
		System.out.println("Using next(): " + intnum + "\n");
		
		System.out.println("\rEnter first name: ");
		String fname = input.next();
		System.out.println("Using next(): " + fname + "\n");
		
		//used new scanner to print the String using nextLine(); in which is repeating
		Scanner newScanner1 = new Scanner(System.in);
		
		System.out.println("\rEnter place: ");
		String testplace = newScanner1.nextLine(); 
		System.out.println("Using nextLine(): " + testplace + "\n");
		
		//print everything
		System.out.println("Using nextLine(): " + value + "\r " + "Using next(): " + fname + "\r " + "Using nextBigInteger(): " + bigInt + "Using nextBigInteger(): " + secondbigInt + "\r " + "Using nextBigDecimal(): " + bigDec + "\r " + testplace + "\r " + doub + "\r " + intnum);
		
		input.close();
	}
}

/*using nextLine(); prints multiple lines of words while next(); only prints a single line of word */
