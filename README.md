# craete-the-pattern-using-java
enter the n 5 11112  32222  33334  54444  55556 


package pattern_visnu;

import java.util.Scanner;

public class vp {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc=new Scanner(System.in);
		System.out.println("enter the n");
		int inc=sc.nextInt();
		int n=inc+1;
		int mat[][]=new int[n][5];
		
		for(int i=1;i<n;i++)
		{
			for(int j=0;j<5;j++)
			{
				if(i%2==0)
				{
					if(j==0)
					{
				       mat[i][j]=i+1;
					}
					else
					{
					mat[i][j]=i;
					}
				}
				else
				{
					if(j==4)
					{
				       mat[i][j]=i+1;
					}
					else
					{
					mat[i][j]=i;
					}
				}
				
			}
		}
		for(int i=1;i<n;i++)
		{
			for(int j=0;j<5;j++)
			{
        System.out.print(mat[i][j]);
        

			}
			System.out.println(' ');
		}
	}

}
