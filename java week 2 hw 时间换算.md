
# 代码
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {

        int BJT, UTC;
        Scanner in = new Scanner(System.in);
        BJT = in.nextInt();
         
        if (0 <= BJT && BJT <= 2359) //范围为0到2359
        {
            if (BJT % 100 <= 59)  //其中百位和个位代表分钟，不超过60; 对100取余，即可得到两位数
            {
                if (BJT >= 800) //如果小时大于8点则可以直接相减 
                {
                   UTC = BJT - 800;
                } 
               else 
                {
                   UTC = 2400 - (800 - BJT);//如果小于8点，减完要倒退到前一天 
                }
            System.out.println(UTC);
                } 
            else 
                {
            System.out.println("错误的输入时间");
                }
        } 
        else
            {
        System.out.println("错误的输入时间");
        }
        
        
    }

}





