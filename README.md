
/*  Simple calculator 
    in this program we create different member method in class 
    to perform calulator operations 

    output:  Enter two number:
              5
              4
         System.out.println("Press 1 for addtion: ");
         System.out.println("Press 2 for subtraction: ");
         System.out.println("Press 3 for multipliction: ");
         System.out.println("Press 4 for divition: ");
         System.out.println("Enter your choice: ");
         1
         Sum: 9
         Press 0 if you want to continue process:
         3
         exit the program

 */

import java.util.Scanner;

class Cal
{
     void sum(float a,float b)
     {
        System.out.println("Sum : "+(a+b));
     }
     void sub(float a,float b)
     {
        System.out.println("Subtration: "+(a-b));
     }
     void mul(float a,float b)
     {
        System.out.println("Multiplication: "+(a*b));
     }
     void div(float a,float b) 
     {
        System.out.println("Division : "+(a/b));
     }
}

public class Calculater
{
    public static void main(String arg[])
    {
         float x,y;
         int n,choice;
         Cal obj=new Cal();
         Scanner sc=new Scanner(System.in);
         do
         {
         System.out.println("Enter two numbers:  ");
         x=sc.nextFloat();
         y=sc.nextFloat();
         System.out.println("Press 1 for addtion: ");
         System.out.println("Press 2 for subtraction: ");
         System.out.println("Press 3 for multipliction: ");
         System.out.println("Press 4 for divition: ");
         System.out.println("Enter your choice: ");
         n=sc.nextInt();
         switch(n)
         {
            case 1:
                obj.sum(x,y);
                break;
            case 2:
                obj.sub(x,y);
                break;
            case 3:
                obj.mul(x,y);
                break;
            case 4:
                obj.div(x,y);
                break;
                 
         }
         System.out.println("Press 0 if you want to continue process: ");
         choice=sc.nextInt();

    }while(choice==0);
}
}
