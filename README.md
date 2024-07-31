# ZEROS-SHOULD-BE-SENT-TO-THE-END-OF-THE-ARRAY
import java.util.*;
class Main {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int [] a=new int[n];
        System.out.println("Enter array elements");
        for(int i=0;i<n;i++){
            int k=sc.nextInt();
            a[i]=k;
        }
        for(int j=0;j<n;j++){
        for(int i=0;i<n-1;i++){
            if (a[i]==0){
                a[i]=a[i+1];
                a[i+1]=0;
            }
        }
        }
        for(int i=0;i<n;i++){
            System.out.print(a[i]+" ");
        }

    }
