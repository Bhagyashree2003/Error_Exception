# Error_Exception
java Error Exception

import java.util.*;
class exception
{
	public static void main(String args[])
	{
		int []mks=new int[6];
		mks[0]=37;
		mks[1]=57;
		mks[2]=74;
		mks[3]=21;
		mks[4]=55;
		mks[5]=45;
		Scanner sc=new Scanner(System.in);
		System.out.println("Enter the array index:");
		int ind=sc.nextInt();
		System.out.println("Enter the number u want to divide the value with:");
		int number=sc.nextInt();

		try
		{
			System.out.println("The value at array index entered is:"+mks[ind]);
			System.out.println("The value of array-value is:" +mks[ind]/number);
		}
		
		catch (ArithmeticException e)
		{
			System.out.println("Arithmetic exception occured!");
			System.out.println(e);
		}
		catch (ArrayIndexOutOfBoundsException e)
		{
			System.out.println("ArrayIndexOutOfBounds exception occured!");
			System.out.println(e);
		}
		catch(Exception e)
		{
			System.out.println("Some exception occured!");
			System.out.println(e);
		}
	}
}
