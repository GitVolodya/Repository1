# Repository1
ITS-b-o-22-1, 11.03.02, Khachatryan Vladimir Vladimirovich

#include <conio.h>
#include <stdio.h>
#include <stdlib.h>
#include <locale.h>
int** input(int n, int m)
{
	setlocale(LC_ALL, "Rus");
	int i, j;
	int** a;
a = (int**)malloc(m * sizeof(int*));
	for (i = 0; i < m; i++)
	{
		a[i] = (int*)malloc(n * sizeof(int*));
		for (j = 0; j < n; j++)
		{
			a[i][j] = 0;
		}
	}


for (i = 0; i < m; i++)
		for (j = 0; j < n; j++)
		{
			printf("\n ¬ведите элемент матрицы A(%d,%d)", i + 1, j + 1);
			scanf_s("%d", &a[i][j]);
		}

