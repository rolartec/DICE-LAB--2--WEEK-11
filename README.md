DICE-LAB--2--WEEK-11
====================

DICE LAB #2 WEEK 11


//   BY REINA OLARTE
//  LAB #2  WEEK #11  "DICE"


public class Dice 
{
	
	//  VARIABLES : 
	
	
	int COMPNumber;
	int ADDNumbers;
	int GENNumber;
	int NUMBbounces;
	int AVENumber;

		public int Throw()
		{
				COMPNumber = (1	 + (int)(Math.random() * 6));
				System.out.printf("The number that the computer generated was %d\n", COMPNumber);
				return COMPNumber;
		}
		public int Throw(int bounces)
		{
			int i=1;
			
			NUMBbounces = bounces;
			
			while(i <= bounces)
			{
				GENNumber = (1+(int)(Math.random() *6));
				
				System.out.printf("The generated number is: %d\n", GENNumber);
				
				ADDNumbers += GENNumber;
				
				System.out.printf("The Sum of the Number: %d\n\n", ADDNumbers);
				
				i++;
			}
			COMPNumber = ADDNumbers / NUMBbounces;
			
			return COMPNumber;
		}
		public int Value()
		
		{
			return COMPNumber;
		}
}
