# BMI-Calculator-Java

import java.util.Scanner;

public class BMICalculator {
	public static void main( String[] args ) {
		Scanner keyboard = new Scanner(System.in);
		double m, in, feet, totalheightinch, kg, lbs, bmi;
		
		System.out.print( "Your height in feet (enter inches separately): " );
		feet = keyboard.nextDouble();
		System.out.print( "and inches: ");
		in = keyboard.nextDouble();
		
		totalheightinch = feet*12 + in;
		
		m = totalheightinch*0.0254;
		
		System.out.print( "Your weight in pounds: " );
		lbs = keyboard.nextDouble();
		
		kg = lbs*0.453592;
		
		bmi = kg / (m*m);
		
		System.out.println( "Your BMI is " + bmi);
		}
		
}
