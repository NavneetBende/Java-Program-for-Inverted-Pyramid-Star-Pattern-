Printing Inverted Pyramid Star Pattern
In this program we’re going to code inverted pyramid pattern program .

Take a input from user as and give him a message as enter the no of lines and then store it in variable n Then run the for loop start from i=n to i– and then take another inner for loop to take j loop start from j=i to j++ and then print space After that take another inner loop start from j=1 to j++ and then print star

Inverted Pyramid Star Pattern
Algorithm:
Enter the number of lines take input from the user and store it in any variable.(‘n‘ in this case).
Run a loop ‘n’ number of times to iterate through each of the rows. From i=n to i>=1. The loop should be structured as for( i=n; i>=1 : i–).
 Run a nested loop inside the main loop to print the spaces before the pyramid. From j=i to j<n. The loop should be structured as for(j=i;j<n;j++)
Inside this loop print white space.
Run another nested loop after the previous loop to print the stars in each column of a row. From     j=1 to j<2*i-1. The loop should be structured as for(j=1;j<=(2*i-1);j++)
Inside this loop print star.
Move to the next line by printing a new line System.out.println(“”);
Code in Java:
import java.util.Scanner;
public class Pattern1 {

	public static void main(String[] args) {
		int i,j,n;
		Scanner sc = new Scanner(System.in);
	     System.out.println("Enter the no of lines");
	     n = sc.nextInt();
		for(i=n;i>=1;i--)
	     {
	         for(j=i;j<n;j++)
	            System.out.print(" ");
	         
	         for(j=1;j<=(2*i-1);j++)
	            System.out.print("*");
	         
	       System.out.println("");
	     } 
	 }

}
