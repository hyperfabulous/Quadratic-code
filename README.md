#include <stdio.h>
#include <stdlib.h>

int main()
{
	float a,b,c,D,X1,X2;
	printf("Enter a,b and c of Quadratic Equation:");
	scanf("%f %f %f", &a,&b,&c);
	
	D =b*b-4*a*c;
	
	if(D<0)
	{
	printf("Roots of Quadratic Equation are:");
	printf("%f%f", -b/(2*a), sqrt(-D)/(2*a));
	printf(",%f%f", -b/(2*a), -sqrt(-D)/(2*a));
	}
	else if(D==0)
	{
	printf("Both Roots Are Equal.\n");
	X1 = -b/(2*a);
	printf("Root Of quadratic Equation is:%f", X1);
	}
	
	else
	// if D > 0 
	{
	printf("Roots Are Real Numbers.\n");
	X1=(-b+sqrt(D))/(2*a);
	X2=(-b-sqrt(D))/(2*a);
	printf("Roots of Quadratic Equation Are:%f, %f",X1,X2);
	}


}
