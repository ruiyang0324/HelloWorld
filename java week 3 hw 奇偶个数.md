



# 代码



import java.util.Scanner;
public class Main {
public static void main(String[] args) {
      
      Scanner in = new Scanner(System.in);
      
      int i = 0, j = 0; //定义两个变量表示奇数和偶数，while循环遍历即可，若偶数则i++，否则j++
       while (true) 
       {
         int a = in.nextInt();
         if ( a==-1) 
         {
          break;
          } 
          else if (a%2 == 0) 
          {
          i++;
          } 
          else 
          {
          j++;
          }
        }
        System.out.println(j + " " + i);
        
    }
}






