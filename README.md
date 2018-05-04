# basiccoding
 basic coding using java
import java.util.*;
public class FutureValue{
	public static void main (String args[]){
		Scanner A = new Scanner(System.in);
		System.out.print("The Starting amount :");
		double a = A.nextDouble();
		System.out.print("The interest rate in percent:");
		double b = A.nextDouble();
		System.out.print("The number of years :");
		int c = A.nextInt();
		if (a>0&&c<=40){
		double Final = a;
		for (int i =1; i <=c ; i++){
			Final = Final + b/100*Final;
		}
		
		System.out.printf("After "+c+" year(s) the amount will be :%.2f\n",Final);
		}
		if (a>0&&c>40){
		System.out.println(c+" years are too long, please make it shorter and then try again");
			
		}
		if(a<=0&&c>40){
			System.out.println("The Starting amount should be positive and "+c+" years are too long, please try a positive starting amount and make years shorter");
		}
		
		
		}
