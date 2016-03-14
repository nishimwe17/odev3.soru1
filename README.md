#include <stdio.h>
#include <stdlib.h>

int main (int argc, char *argv[])
{
	int i;
	i = atoi(argv[1]);
	if (i == 1)
	sifrele();
	else if (i == 0) 
	sifrecoz();	
}
	
int sifrele()
{
	int c;
	c = getchar();
	while (c !=EOF){
	c = c + 6;
	putchar(c);
	c = getchar();
	}
	return 0;
}

int sifrecoz()
{
	int c;
	c = getchar();
	while (c !=EOF){
	c = c - 6;
	putchar(c);
	c = getchar();
	}
	return 0;
}
