import java.util.*;

public class Test{

    public static void main(String []args){
        int n,i,j,k=0;
        n = 4 ;
        for(i=1;i<=n;i++) {
            for(j=1;j<=(2*n)-i;j++) {//(2*n)-i  is number columns for each row
                if(j<=n-i) {        //print the spaces
                    System.out.print(" ");
                } else if(i%2==1) { //print the odd rows
                    k++;
                    System.out.print(k+" ");
                } else {                //print the even rows
                    System.out.print(k+" ");
                    k--;             //decrement the values
                }
            }k+=n;                   //starting value for each row
            System.out.print("\n");
        }
    }
}