# meghana
Income Tax Calculator
import java.util.Scanner; //Needed for Scanner class import java.lang.Math; public class CretsingerCatherineTaxCalculator { public static void main(String[] args) { Scanner keyboard = new Scanner(System.in); //Scanner object for keyboard input int single; int income = 0; double tax1;
double tax2; double tax3; double tax4; double tax5; double tax6; final double tax_one = .10; final double tax_two = .15; final double tax_three = .25; final double tax_four = .15; final double tax_five = .25;
//Ask the user if single or married System.out.print("Are you single or married? Enter 0 for single or 1 for married "); //Get status from user single = keyboard.nextInt();
if (single == 0) { System.out.println("What is your taxable income?"); income = keyboard.nextInt(); }
else if (single == 1) { System.out.println("What is your taxable income?"); income = keyboard.nextInt(); } tax4 = (tax_one * income); tax5 = (tax_four * income) + 1600; tax6 = (tax_five * income) + 8800; if(income >= 0 && income < 16000) { System.out.println("The amount of taxes you must pay is " + tax4); }
else if (income >= 16000 && income < 64000) { System.out.println("The amount of taxes you must pay is " + tax5); } else if (income >= 64000) { System.out.println("The amount of taxes you must pay is " + tax6); tax1 = (tax_one * income); tax2 = (tax_two * income) + 800; tax3 = (tax_three * income) + 4400;
if (income >= 0 && income < 8000) {
System.out.println("The amount of taxes you must pay is " + tax1);
}
else if (income >= 8000 && income < 32000) {
System.out.println("The amount of taxes you must pay is " + tax2);
}
else if (income >= 32000) {
System.out.println("The amount of taxes you must pay is " + tax3);
}
}
}
}
Sample output
Are you single or married? Enter 0 for single or 1 for married 0 What is your taxable income? 52000 The amount of taxes you must pay is: 9400
