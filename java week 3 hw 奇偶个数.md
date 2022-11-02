



# 代码



import java.util.Scanner;
public class Main {
public static void main(String[] args) {
      Scanner in = new Scanner(System.in);
      //定义两个变量表示奇数和偶数，while循环遍历即可，若偶数则i++，否则j++
        int j = 0, i = 0;
        while (true) {
           int a = in.nextInt();
            if ( a==-1) {
                break;
            } else if (a%2 == 0) {
                i++;
            } else {
                j++;
            }
        }
        System.out.println(j + " " + i);
    }
}



# eclipse练习



