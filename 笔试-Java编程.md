<h3>笔试-Java编程题</h3>
1.打印当前时间：

	import java.util.Date;
	import java.text.SimpleDateFormat;
	 
	public class Main {
	    public static void main(String[] args) {
	        Date now = new Date();
	        SimpleDateFormat simpleDateFormat = new SimpleDateFormat("yyyy/MM/dd HH:mm:ss");
	        System.out.println(simpleDateFormat.format(now));
	    }
	}


2.判断一个数是否是2的幂

	public boolean check(int num){
        int temp = fuc(num);
        boolean result = (temp == 1 );
        return result;
    }
	public int fuc(int num){
        if(num % 2 == 1) {
            return 0;
        }else if(num == 2){
            return 1;
        }else{
            return fuc(num / 2);
        }
    }