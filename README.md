package shabby;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
	 int firstNumber,secondNumber,result,choice;
        System.out.println("_____Calculator Menu_____");
        System.out.println("1.Addition");
        System.out.println("2.Subtraction");
        System.out.println("3.Multiplication");
        System.out.println("4.Division");
        System.out.println("__________________________");
        Scanner scanner=new Scanner(System.in);
        System.out.print("Enter the numbers: ");
        firstNumber= scanner.nextInt();
        secondNumber=scanner.nextInt();
        System.out.print("Enter your choice:");
        choice=scanner.nextInt();

        switch (choice){
            case 1:
                result=firstNumber+secondNumber;
                System.out.print("Addition of two numbers is :"+result);
                break;
            case 2:
                result=firstNumber-secondNumber;
                System.out.print("Subtraction of two numbers is :"+result);
                break;
            case 3:
                result=firstNumber*secondNumber;
                System.out.print("Multiplication of two numbers is :"+result);
                break;
            case 4:
                if(secondNumber!=0){
                    result=firstNumber/secondNumber;
                    System.out.print("Division of two numbers is :"+result);
                }
                else {
                    System.out.print("Cannot divide by zero ");
                }
                break;
            default:
                System.out.println("Invalid choice");
                break;
        }
    }
}
