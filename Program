import java.util.Scanner;
public class Q5_Roman2Integer {

    public static void numberConverter(String x){ // Subroutine to convert Roman numeral to numerical value

        // Declaring and initializing variables
        int roman_X = 0;
        int roman_I = 0;
        int roman_V = 0;
        int roman_L = 0;
        int roman_C = 0;
        int roman_D = 0;
        int roman_M = 0;
        int ans = 0;
        String initial_value = x;
        int num2 = 0;


        // Identifying special cases of from the input
        while (x.contains("IV") || x.contains("IX") || x.contains("XL") || x.contains("XC") || x.contains("CD") || x.contains("CM")){

            // Removing special cases from string
            if ((x.contains("IV"))){
                num2 = num2 + 4;
                x = x.replace("IV", "");
            }
            if (x.contains("IX")) {
                num2 = num2 + 9;
                x = x.replace("IX", "");
            }
            if (x.contains("XL")){
                num2 = num2 + 40;
                x = x.replace("XL", "");

            } if (x.contains("XC")){
                num2 = num2 + 90;
                x = x.replace("XC", "");

            } if (x.contains("CD")){
                num2= num2 + 400;
                x = x.replace("CD", "");

            } if (x.contains("CM")){
                num2 = num2 + 900;
                x = x.replace("CM", "");

            }

        }

        // Iterating through the remainder of the string
        for (int i = 0; i < x.length(); i++) {

            //Keeping track of the instances of each symbol
            char digit = x.charAt(i);

            if (digit == 'X') {
                roman_X++;

            } else if (digit == 'I') {
                roman_I++;

            } else if (digit == 'V') {
                roman_V++;

            } else if (digit == 'L') {
                roman_L++;
            } else if (digit == 'C') {
                roman_C++;

            } else if (digit == 'D') {
                roman_D++;

            } else if (digit == 'M') {
                roman_M++;
            }
        }

        // Computing calculations
        roman_X = (roman_X) * 10;
        roman_I = (roman_I) * 1;
        roman_V = (roman_V) * 5;
        roman_L = (roman_L) * 50;
        roman_C = (roman_C) * 100;
        roman_D = (roman_D) * 500;
        roman_M = (roman_M) * 1000;

        // Adding all values to obtain corresponding integer
        ans = num2 + roman_X + roman_I + roman_V + roman_L + roman_C + roman_D + roman_M;

        // Printing corresponding integer
        System.out.println(initial_value + " -> " + ans);

    }

    public static void main(String[] args){

        // Creating Scanner
        Scanner user_input = new Scanner(System.in);

        // Asking for user input of Roman numeral
        System.out.println("Enter number in Roman Numerals (e.g II): ");
        String input = user_input.nextLine();


        // Calling subroutine to convert input to corresponding integer number
        numberConverter(input);

    }
}
