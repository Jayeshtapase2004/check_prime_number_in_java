package EXAMPLES; // package name it cqan be any thing is is just your folder for workspace
import java.util.Scanner;
//importing Scanner Class from java.util package(predefined folder in JDK) to get input from the user
public class Prime   { //creating A class name "Prime"
    public static void main(String[] args) { //declaring main in the class
           int num,count=0,i;//Creating different variable of int datatype

        Scanner Jay= new Scanner(System.in);// Creating an object to access the Scanner class for taking input from the keyboard
        System.out.println("Enter an integer:");//Displaying necessary details to the user
        num=Jay.nextInt();
        /*here we are assigning the value of the input number given by the user to a variable "num"
         from the object "Jay" and nextInt() method returns the int value scanned from the input.
         */
        for(i=1;i<=num;i++) // giving the test conditions in the for loop to check the prime number
        {
            if(num%i==0) // it defines if the value of num variabe is divided by the value of i which is continuosly incrementing is 0 move to the code inside this if.
                count++; //if the statement comes true then increment the value of count variable.
        }
        if(count>2)// if the value of count is more than 2 the move to the  statement of the if.
            System.out.println("number "+num+" is not prime");//display the reasult to the user
        else// if the value of if condition becomes false then move to this statement
            System.out.println("number "+num+" is prime");//display the reasult to the user
    }
}

