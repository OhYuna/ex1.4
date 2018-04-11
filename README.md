#include <stdio.h>

int main(void)
{
	int a;
	int fac;
	int sum = 0;
	int n;

	for (a = 1; a <= 10; a++) {
		fac = 1;
		n = 1;

		do{
		fac *= n;
		n++;
		} while (n <= a);

		if(a != 10)
			printf("%d! + ", a);
		else
			printf("%d! \n", a);

		sum += fac;
	}

	printf(" = %d \n", sum);
}
