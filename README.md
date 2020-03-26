## Codezz Corner C@|]ES
## Digital Pattern
    import java.util.Scanner;
    public class Main {
        public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int m=sc.nextInt();
        int N=sc.nextInt();   //N is always odd
        for(int i=0;i<N;i++){ 
            for(int j=0;j<N;j++){
               //upper
               if((m==0 || m==2 || m==3 || m==4 || m==5 || m==6 || m==7 || m==8 || m==9) && (i==0)){
               System.out.print(m);
               }
               //middle
               else if((m==2 || m==3 || m==4 || m==5 || m==6 || m==8 || m==9) && (i==N/2)){
               System.out.print(m);
               }
               //lower
               else if((m==0 || m==2 || m==3 || m==5 || m==6 || m==8 || m==9) && (i==N-1)){
               System.out.print(m);
               }
               //left1
               else if((m==0 || m==4 || m==5 || m==6 || m==8 || m==9) && (i<N/2 && j==0)){
               System.out.print(m);
               }
               //left2
               else if((m==0 || m==2 || m==6 || m==8) && (i>N/2 && j==0)){
               System.out.print(m);
               }
               //right1
               else if((m==0 || m==1 || m==2 || m==3 || m==4 || m==8 || m==9) && (i<N/2 && j==N-1)){
               System.out.print(m);
               }
               //right2
               else if((m==0 || m==1 || m==3 || m==4 || m==5 || m==6 || m==7 || m==8 || m==9) && (i>N/2 && j==N-1)){
               System.out.print(m);
               }
               else{
               System.out.print("*");
               }
            }
            System.out.println(); 
        }  }  }
        
   INPUT : 5 7
          
   OUTPUT :
   
         5555555
         5******
         5******
         5555555
         ******5
         ******5
         5555555
         
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
