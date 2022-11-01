# 代码

import java.util.Scanner;

public class Hello {
	

	public static void main(String[] args) {
		
		int rs;
		Scanner in = new Scanner(System.in);
		rs = in.nextInt();
		int s =rs%10;
		int r = rs/10%10;
		//r为十位数；s为个位数；用Switch-case语句输出；注意使用Break
		if (r>=1 && r<=5 && s>=1 && s<=9) {
			switch (s){
			case 1:System.out.println("Faint signals, barely perceptible"+", ");
			       break;
			case 2:System.out.println("Very weak signals"+", ");
		       break;    
			case 3:System.out.println("Weak signals"+", ");
		       break;
			case 4:System.out.println("Fair signals"+", ");
		       break;
			case 5:System.out.println("Fairly good signals"+", ");
		       break;
			case 6:System.out.println("Good signals"+", ");
		       break;
			case 7:System.out.println("Moderately strong signals"+", ");
		       break;
			case 8:System.out.println("Strong signals"+", ");
		       break;
			case 9:System.out.println("Extremely strong signals"+", ");
		       break;
			}
			
			switch (r){
			case 1:System.out.println("unreadable"+".");
			       break;
			case 2:System.out.println("barely readable, occasional words distinguishable"+".");
		       break;    
			case 3:System.out.println("readable with considerable difficulty"+".");
		       break;
			case 4:System.out.println("readable with practically no difficulty"+".");
		       break;
			case 5:System.out.println("perfectly readable"+".");
		       break;
			}
		}
		else {
			System.out.println("no!");
		}

   }
	
}




