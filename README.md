## Codezz-Corner C@|]ES
## Astreik Pattern
    import java.util.Scanner;
    public class Main {
        public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int d=sc.nextInt();
        String s=sc.next(); 
        int len=s.length();
        int x=d-1,y=d-1,k=1; 
        for(int i=0;i<n;i++){ 
            x=d-(i+1); y=d-1; 
            int j=0;
            while(j<len){
                if(j>=x && j<y){ 
                    System.out.print("*");
                }
                else if(j==y){
                    System.out.print("*");
                    x=x+n;
                    y=y+n;
                }
                else{ 
                    System.out.print(s.charAt(j));
                } 
                j++;
            } 
            System.out.println(); 
        }  } }
        
   INPUT : 
   
          3
          CRATMATES
          
   OUTPUT :
   
         CR*TM*TE*
         C**T**T**
         *********
