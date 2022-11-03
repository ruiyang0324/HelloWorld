

# 代码

public class Hello {
	
	public static void main(String[] args) {


		 Scanner in = new Scanner(System.in);
	        int number = in. nextInt(); 
	        int a = 0; // a表示number的数位
	        int b = 0; // b表示number的数字
	        int c = 1; // c表示二进制的数值为1
	        int result =0;   
	        while (number != 0) {
	        	b = number % 10; //得到尾数
	            number = number / 10;  //去掉当前尾数，方便下一轮运算
	            a++;  //数位加一
	            if ((b%2==0&&a%2==0)||(b%2!=0&&a%2!=0)) 
	            //判断是否满足条件;a与b奇偶性相同
	            {
	            	result+= c;  //累加计算
	            }
	            c=2*c;
	        }
	        System.out.println(result);
		}

	}







