# look
laba
#include "pch.h"
#include <iostream>
#include <stdio.h>
using namespace std;

int main()
{
	int m, m1, i = 0;
	int n, n1, n2;
	int reshenie[20];
	printf("Napishi chislo m?\n");
	scanf_s("%d", &m);
	m1 = m;
	for (int y = m; y > 0; y--)
	{
		bool k=true;
		m1 = y;
		while (m1)
		{
			n = m1 % 2;
			m1 = m1 / 2;
			reshenie[i] = n;
			if (reshenie[i] == 0)
				k = false;
			i++;
		}
		if (k)
		{
			printf("\n%d-", y);
			for (int l = 0; l < i; l++)
				printf("%d", reshenie[i]);
		}

		i = 0;
		
	}

	return 0;
}

