# Lab-Test

> x Questions will be given on the day of the test.

> Pick question according to your roll number: 
  for e.g if x=4 and last three digit of your roll no are 123 then your question no is (1+2+3)%4 + 1 = 3
  
# Pull this repository and Fill in the blanks in Readme File alongwith:

Name: Sandeep Choudhary
Roll No:143
SAPID: 500064341
Batch:B3
Question Assigned: 3,4


# How to code?

* Use proper coding ethics.
* Use Package.
* Use Access Modifiers Properly.
* Different file for each class.
* Folder hierachy: 
                  src/com/bao/<your_roll_no>/<your_class.java>
                  bin/com/bao/<your_roll_no>/<your_class.class>
                  
* To do all above Code in Eclipse and commit in your own repository you pulled earlier.
* Raise a merge request(thru github webpage) to me and add screenshot of output withit.
* Request should be raised within Lab timing. i.e 

              # B4 BAO - 15 April 2019 11:30-13:30Hrs
              # B3 BAO - 16 April 2019 09:30-11:30Hrs
              # B3 OGI - 17 April 2019 09:30-11:30Hrs
              
              MAX Allowable time with marks deduction is 1 Hour.
              
All the Best!!
Q1
 package testlab;

public class Testq1 {
	
  public boolean inorderEqual(int a,int b,int c, boolean equalok)
  {  if(b>a && c>b) 
    {
	  return true;
     }
	  else if(equalok&& (a<=b && b<=c))
	  {
		    return true;
	  }
	  else if((a<=b && b<=c) &&!equalok) {
		  return true;
	  }
		  else
		    return false;
		    
    
  
	  }
  public static void main(String[] args) {
     boolean e;
	  Testq1 a=new Testq1();
       e=a.inorderEqual(5, 5, 7, false);
       System.out.println(e);
     
}
}
Q2
package testlab;

public class Testq2 {

	public boolean makeBricks(int small, int big, int goal)
	{
		int maxBig = goal/5;
		if(maxBig <= big)
			goal -= maxBig*5;
		else
			goal -= big*5;
		if(goal <= small)
			return true;
		else
		return false;
	}
	public static void main(String args[])
	{
		boolean d;
		Testq2 b=new Testq2();
		d=b.makeBricks(1, 5, 3);
		System.out.println(d);
	}

}




