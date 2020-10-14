package assignment.OOP;
 
import javax.swing.*;
import java.util.Scanner;
 
public class Kalkulator1
{
    public static void main(String[] args)
    {
        Scanner id = new Scanner (System.in);
        int numb1, numb2;
        System.out.println("Menu:");
        System.out.println("1. subtractNumbers");
        System.out.println("2. multiplyNumbers");
        System.out.println("3. divisionNumbers");
        String data_pilihan = JOptionPane.showInputDialog("choose (1-3) :");        
        int pilihan = Integer.parseInt(data_pilihan);
        System.out.println("input numb1 :");
        numb1 = id.nextInt();
        System.out.println("input numb2 :");
        numb2 = id.nextInt();                
        switch (pilihan)
        {
            case 1:
            {
                int substract = numb1-numb2;
                System.out.println("substractNumbers " +numb1+ " - " +numb2+ " = "+substract);
                break;
            }
            case 2:
            {
                int multiply = numb1*numb2;
                System.out.println("multiplyNumbers " +numb1+ " * " +numb2+ " = "+multiply);
                break;
            }
            case 3:
        {
                int divison = numb1/numb2;
                System.out.println("divisionNumbers " +numb1+ " : " +numb2+ " = "+division);
                break;
            }
            default:
                System.out.println("failed");
                break;
        }
    }
}
