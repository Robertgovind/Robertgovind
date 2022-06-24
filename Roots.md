//to find the roots of quadratic equation.
#include<stdio.h>
#include<conio.h>
#include<math.h>
int main()
{
	int a,b,c;
	float x1,x2,d,d1,real,img;
	printf("Suppose the equation ax^2+bx+c");
	printf("\n Enter the values of a,b&c:\t");
	scanf("%d%d%d",&a,&b,&c);
	d1=(b*b-4*a*c);
if(d1<0)
	{
		d=sqrt(-d1); // sir lai fabs() ko function sodhnu xa
		real=-b/2*a;
		img=d/2*a;
		printf("\nThe imaginary roots are:");
		printf("\n x1=%.2f+%.2fi \t x2=%.2f-%f.2fi",real,img,real,img);
		
		}
	else 
	{
		d=sqrt(d1);
	x1=(-b+d)/2*a;
	x2=(-b-d)/2*a;
	printf("\nThe first root is x1=%.2f",x1);
	printf("\n Thge second root is x2 = %.2f",x2);

		}
			return 0;
	
	}
