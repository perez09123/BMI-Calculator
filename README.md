import java.util.Scanner;

public class BMIcalculator { public BMIcalculator() { }

public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);
    System.out.println("Enter your height in meters: ");
    double height = scanner.nextDouble();
    System.out.println("Enter your weight in kilograms: ");
    double weight = scanner.nextDouble();
    double bmi = weight / (height * height);
    System.out.println("Your BMI is: " + bmi);
    if (bmi < 18.5) {
        System.out.println("Underweight");
    } else if (bmi >= 18.5 && bmi < 25.0) {
        System.out.println("Normal weight");
    } else if (bmi >= 25.0 && bmi < 30.0) {
        System.out.println("Overweight");
    } else if (bmi >= 30.0 && bmi < 35.0) {
        System.out.println("Moderately obese");
    } else if (bmi >= 35.0 && bmi < 40.0) {
        System.out.println("Severely obese");
    } else {
        System.out.println("Very severely obese");
    }

}
}
