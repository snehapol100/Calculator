import java.lang.*;
import java.util.*;
public class Calculator
{
    public static void main(String [] args)
    {
        int N1 = 0, N2 = 0, Res = 0, Choice = 0;
        Scanner Sc = new Scanner (System.in);

        while( true )
        {
            System.out.print("\n==========*****==========\n");

            System.out.print("\n ***** Calculator ***** \n");
            System.out.print("\n Choices : ");
            System.out.print("\n\t 1. Addition ");
            System.out.print("\n\t 2. Subtraction ");
            System.out.print("\n\t 3. Multiplication ");
            System.out.print("\n\t 4. Division ");
            System.out.print("\n\t 5. Remainder ");
            System.out.print("\n\t 6. Exit ");

            System.out.print("\n==========*****==========\n");

            System.out.print("\n Select Your Choice : ");
            Choice = Sc.nextInt();

            if( ( Choice > 0 ) && ( Choice < 6 ))
            {
                System.out.print("\n Enter 1st Number : ");
                N1=Sc.nextInt();
                System.out.print("\n Enter 2nd Number : ");
                N2=Sc.nextInt();                
            }

            switch( Choice )
            {
                case 1 :
                         Res = N1 + N2 ;
                         System.out.print("\n Addition of " + N1 + " & " + N2 + " is = " + Res + ".");
                         Sc.next();
                         break;

                case 2 :
                         Res = N1 - N2 ;
                         System.out.print("\n Subtraction of " + N1 + " & " + N2 + " is = " + Res + ".");
                         break;

                case 3 :
                         Res = N1 * N2 ;
                         System.out.print("\n Multiplication of " + N1 + " & " + N2 + " is = " + Res + ".");
                         break;

                case 4 :
                         Res = N1 / N2 ;
                         System.out.print("\n Division of " + N1 + " & " + N2 + " is = " + Res + ".");   
                         break;         
                         
                case 5 :
                         Res = N1 % N2 ;
                         System.out.print("\n Addition of " + N1 + " & " + N2 + " is = " + Res + ".");
                         break;

                case 6 :
                         break;

                default :
                         System.out.print("\n Invalid Input!!!");
            }

            if( Choice == 6 )
            {
                break;
            }
        } 
        System.out.print("\n Thanks For Using this Calculator Service...\n ");
    }
}
