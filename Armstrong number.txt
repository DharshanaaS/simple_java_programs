package armstrong;
import java.util.Scanner;
public class Armstrong {
    public static void main(String[] args) {
      Scanner obj=new Scanner(System.in);
      System.out.println("Enter any number:");
      int n=obj.nextInt();
      int tot=0,dig,cube;
      while(n>0){
      dig=n%10;
      cube=dig*dig*dig;
      tot=tot+cube;
      n=n/10;
      }
      if(n==tot)
      System.out.println("It is Armstrong number");    
      else
      System.out.println("It is not an Armstrong number");       
 }
} 
