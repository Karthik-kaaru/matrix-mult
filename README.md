# matrix-mult
to create matix add nd multipliaction
package matrix;
import java.util.*;
public class MatrixAddMul {

	public static void main(String[] args) {
		int a[][]= {{1,3,4},{2,4,3},{3,4,5}};
		int b[][]= {{1,3,4},{2,4,3},{1,2,4}};
       int add[][]=new int[3][3];
       int mul[][]=new int[3][3];
        int sum1;
        sum1=0;
        for(int i=0;i<3;i++)
        {
        	 for(int j=0;j<3;j++)
             {
              add[i][j]=a[i][j]+b[i][j];
             }
        }
         System.out.println("Addtion is ");
        for(int i=0;i<3;i++)
        {
        	 for(int j=0;j<3;j++)
             {
      
       System.out.print(add[i][j]+" ");
         }
         System.out.println();
        }
        for(int i=0;i<3;i++)
        {
        	 for(int j=0;j<3;j++)
             {
        		 for(int k=0;k<3;k++)
        		 {
              sum1=sum1+a[i][k]*b[k][j];
     	}
        	 mul[i][j]=sum1;
        }
        }
        System.out.println("Multiplication is ");
        for(int i=0;i<3;i++)
        {
        	 for(int j=0;j<3;j++)
             {
       System.out.print(mul[i][j]+" ");
             }
             System.out.println();
        }

}
}
