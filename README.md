import java.util.Scanner; 
 
class Main { 
    public static void main(String[] args) { 
        Scanner sc = new Scanner(System.in); 
        int count=0; 
        int n=sc.nextInt(); 
        int d=sc.nextInt(); 
        Long[] a = new Long[n]; 
        for(int i=0;i<n;i++) 
        { 
            a[i]=sc.nextLong(); 
        } 
 
        for(int i=0;i<n;i++) 
        { 
            if(a[i] > 10) 
            { 
               Long t=a[i]%100; 
               if((t/10) == d) 
                   { 
                       count++; 
                   }     
           } 
        } 
        System.out.println(count); 
         
     
    } 
}
